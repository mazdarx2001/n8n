---

tags:
  - Workflow²

---

# Looping in Workflow²

Looping enables you to repeatedly perform the same actions, stopping only after a set number of repetitions (e.g. fetch the 10 most recent items) or when a specific condition is met (e.g. no new items exist).

Looping is useful when you want to process multiple similar items, for example sending a message to every contact in your address book. In Doc² this repetitive processing is handled automatically, meaning you do not need to specifically build loops into your workflows. There are some [special cases](#node-exceptions) where this isn’t true.

## Using loops in Workflow²

Workflow² nodes take any number of items as input, process these items, and output the results. You can think of each item as a single data point (or a single row in the output table of a node).

The following image shows the output from the [Customer Datastore](/workflow/integrations/nodes/workflow-nodes-base.TrainingCustomerDatastore/) node, where each row is an individual item.

![The Customer Datastore node](/_images/flow-logic/looping/customer_datastore_node.png)

**Nodes usually run once for each item**. For example, if you want to send the name and notes of the customers as a message on [Slack](/workflow/integrations/nodes/workflow-nodes-base.slack/), connect the Slack node to the Customer Datastore node, configure the parameters, and execute the node. You will receive 5 messages — one for each item.

This is how you can process multiple items without having to explicitly connect nodes in a loop.

!!! note " Keep in mind"
    Your data must be in the proper structure for Doc² to process it as described here. See [Transforming Data](/workflow/data/transforming-data/) to learn more.


### Executing nodes once

For situations where you do not want a node to process all received items, for example sending a Slack message only to the first customer, you can do so by toggling the **Execute Once** parameter in the *Settings* tab of that node.

This setting is helpful when the incoming data contains multiple items and you want to only process the first one. Using the [Customer Datastore](/workflow/integrations/nodes/workflow-nodes-base.workflowTrainingCustomerDatastore/) and [Slack](/workflow/integrations/nodes/workflow-nodes-base.slack/) example from above, it would look like the following:

![Execute once enabled for the Slack node](/_images/flow-logic/looping/execute_once.png)

You can see a message was sent only for the first customer - Jay Gatsby.

### Executions indicator

When you execute a node a green number gets displayed on its icon. This number represents the number of times the node has executed, it **doesn't** represent the number of items returned by the node. Each execution may return multiple items.

![The executions indicator.](/_images/flow-logic/looping/executions_indicator.png)

If a node receives input from multiple nodes, it will execute separately for each set of input data. For example, if the above node has two input nodes, it will execute twice, once for each input as pictured below.

![Node taking inputs from two different nodes](/_images/flow-logic/looping/multiple_inputs.png)

**Note**: The only exception to this is the [Merge](/workflow/integrations/core-nodes/workflow-nodes-base.merge/) node.

In the above image, notice that the Customer Datastore node gets executed twice, once for each input. To view the output for each input node, select the execution from the **Data of Execution** dropdown list:

![Node output for inputs from two different nodes](/_images/flow-logic/looping/multiple_outputs.png)

When you have a loop in a workflow, the node gets executed multiple times. The number on the node will represent the total number of executions:

![Number of executions of a node in a loop](/_images/flow-logic/looping/loop_executions.png)

## Creating loops

As discussed above, Doc² typically handles the iteration for all incoming items. However, there are certain scenarios where you will have to create a loop to iterate through all items. You can learn more about these [here](#node-exceptions).

To create a loop in an Doc² workflow, connect the output of one node to the input of a previous node. Make sure you add an [IF](/workflow/integrations/core-nodes/workflow-nodes-base.if/) node to check when to stop the loop. You now have a loop that iterates over each item.

Here is an [example workflow](https://workflow.io/workflows/1130) that implements a loop with an `IF` node:

![Editor UI view of sample workflow](/_images/flow-logic/looping/example_workflow.png)

You should use the [Split In Batches](/workflow/integrations/core-nodes/workflow-nodes-base.splitInBatches/) node when you want to batch the data in groups and process these batches. This approach is useful for avoiding API rate limits when processing large incoming data or when you only want to process a specific group of returned items.

**Note**: The Split In Batches node stops executing after all the incoming items get divided into batches and passed on to the next node in the workflow so it is not necessary to add an IF node to stop the loop.

## Node exceptions

There are a limited number of nodes and operations where you need to design a loop into your workflow:

* [**Airtable**](/workflow/integrations/nodes/workflow-nodes-base.airtable/) node:
	* **List**: This operation executes only once, not for each incoming item.
* [**Coda**](/workflow/integrations/nodes/workflow-nodes-base.coda/) node:
	* **Get All**: For the Table and View resources, this operation executes only once.
* [**CrateDB**](/workflow/integrations/nodes/workflow-nodes-base.crateDb/) node will execute and iterate over all incoming items only for Postgres related functions (e.g. `pgInsert`, `pgUpdate`, `pqQuery`).
* [**Execute Workflow**](/workflow/integrations/core-nodes/workflow-nodes-base.executeWorkflow/) node executes only once by default.
* [**Function**](/workflow/integrations/core-nodes/workflow-nodes-base.function/) node processes all the items based on the entered code snippet, but it gets executed only once. If you need to execute the Function node multiple times you have to create a loop using the [Split In Batches](/workflow/integrations/core-nodes/workflow-nodes-base.splitInBatches/) node.
* [**Google Cloud Firestore**](/workflow/integrations/nodes/workflow-nodes-base.googleCloudFirestore/) node:
	* **Get All**: For the Collection and Document resources, this operation executes only once.
* [**Google Drive**](/workflow/integrations/nodes/workflow-nodes-base.googleDrive/) node:
	* **List**: This operation executes only once, not for each incoming item.
* [**Google Sheets**](/workflow/integrations/nodes/workflow-nodes-base.googleSheets/) node:
	* **Read**: This operation executes only once for the `Sheet` resource.
	* **Update**: This operation updates multiple rows if they are in the same range. It does not iterate through additional ranges.
* [**HTTP Request**](/workflow/integrations/core-nodes/workflow-nodes-base.httpRequest/) node: You must handle pagination yourself. If your API call returns paginated results you must create a loop to fetch one page at a time.
* [**Microsoft SQL**](/workflow/integrations/nodes/workflow-nodes-base.microsoftSql/) node does not natively handle looping, so if you want the node to process all incoming items you must create a loop.
* [**Postgres**](/workflow/integrations/nodes/workflow-nodes-base.postgres/) node will execute and iterate over all incoming items only for Postgres related functions (for example, `pgInsert`, `pgUpdate`, `pqQuery`).
* [**QuestDB**](/workflow/integrations/nodes/workflow-nodes-base.questDb/) node will execute and iterate over all incoming items only for Postgres related functions (e.g. `pgInsert`, `pgUpdate`, `pqQuery`).
* [**Read Binary Files**](/workflow/integrations/core-nodes/workflow-nodes-base.readBinaryFiles/) node will fetch the files from the specified path only once. This node doesn’t execute multiple times based on the incoming data. However, if the path is referenced from the incoming data, the node will fetch the files for all the valid paths.
* [**Redis**](/workflow/integrations/nodes/workflow-nodes-base.redis/) node:
	* **Info**: This operation executes only once, regardless of the number of items in the incoming data.
* [**RSS**](/workflow/integrations/core-nodes/workflow-nodes-base.rssFeedRead/) nodes executes only once regardless of the number of items in the incoming data.
* [**Spreadsheet**](/workflow/integrations/core-nodes/workflow-nodes-base.spreadsheetFile/) node processes all the incoming data and creates a single file with all the incoming data. If you want to create individual files for each incoming item, you have to create a loop.
* [**TimescaleDB**](/workflow/integrations/nodes/workflow-nodes-base.timescaleDb/) node will execute and iterate over all incoming items only for Postgres related functions (e.g. `pgInsert`, `pgUpdate`, `pqQuery`).
