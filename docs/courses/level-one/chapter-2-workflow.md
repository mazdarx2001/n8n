# Building the main workflow

[[toc]]

First of all, let’s set up the scene for building Nathan’s workflow. Open your Editor UI and create a new workflow with one of the two possible commands:

- Click **Ctrl + Alt + N** or **Cmd + Alt + N** on your keyboard
- Open the left menu and click on *New* under the Workflow section

Name this new workflow “Nathan’s workflow”.

## 1. Getting data from the data warehouse

The first step we need to take is to get data from Evil Corp’s old data warehouse. 

In the previous chapter, we used a regular node for a specific app (Hacker News). However, not all apps or services have dedicated nodes – like the legacy data warehouse from Nathan’s company. Nathan mentioned that it’s not possible to directly export the data, however the data warehouse has a couple of API endpoints.

That’s all we need to access the data via the [***HTTP Request node***](https://docs.n8n.io/nodes/n8n-nodes-base.httpRequest/)in n8n.

::: tip 💡 No node for that service?
The *HTTP Request node* is one of the most versatile nodes, allowing you to make HTTP requests which can be used to query data from apps and services. You can use it to access data from apps or services that don’t have a dedicated node in n8n.
:::

Now, in your Editor UI, add an *HTTP Request node*, like you learned in the [lesson *Adding nodes*](./chapter-1-components.md#adding-nodes). The node window will open, where you need to configure some parameters.

<figure><img src="./images/chapter-two/HTTP-request-node.png" alt="HTTP Request node" style="width:100%"><figcaption align = "center"><i>HTTP Request node</i></figcaption></figure>


In the left panel, select:

- *Authentication:* Header Auth
- *URL:* https://internal.users.n8n.cloud/webhook-test/custom-erp
- *Options > Add Option > Split Into Items:* toggle to true.  
This option will output each element of an array as its own item.
- *Headers > Add Header:*
  - *Name:* email
  - *Value:* your_address@mail.com

Since you selected *Header Authentication*, now you need to enter your [credentials](https://docs.n8n.io/reference/glossary.html%23credentials), in order to be able to access the data.

::: tip 📖 Credentials
Credentials are unique pieces of information that identify a user or a service and enable them to access apps or services (in our case, represented as n8n nodes). A common form of credentials is a pair of a username and a password, but they can take other forms depending on the service.
:::

Go to the top parameter *Credentials* and click on the pencil icon on the right of the field. This will open the Credentials window, where you need to add information to three fields:

- *Credentials Name:* beginner_course  
You can name your credentials however you want. It’s good practice to give them descriptive names for the app/service, type, and purpose of the credential. A naming convention will make it easier for you to keep track of and identify your credentials.
- *Name:* `api_key`
- *Value:* `"j[vKYdY68H(:WFb`

Your *Credentials* window should look like this:

<figure><img src="./images/chapter-two/HTTP-credentials.png" alt="HTTP Request node credentials" style="width:100%"><figcaption align = "center"><i>HTTP Request node credentials</i></figcaption></figure>

Now click the *Save* button in the bottom right corner of the window.

In the *HTTP Request node* window, click the *Execute Node* button. The result of the HTTP request should look like this:

<figure><img src="./images/chapter-two/HTTP-Request-window.png" alt="HTTP Request node window" style="width:100%"><figcaption align = "center"><i>HTTP Request node window</i></figcaption></figure>

This view should be familiar to you from the [Hacker News mini-workflow](./chapter-1-miniworkflow.md). This is the data from Nathan’s data warehouse that he needs to work with. His data set includes sales information of 30 customers with 5 features:

- *orderID:* the unique id of each order.
- *customerID:* the unique id of each customer.
- *employeeName:* the name of Nathan’s colleagues who are responsible for each client.
- *orderPrice:* the total price of the customer’s order.
- *orderStatus:* whether the customer’s order is booked or still in processing.

----

**Nathan 🙋**: This is great! You already automated an important part of my job with only a couple of clicks. Now instead of manually accessing the data every time I need it, I can use this workflow to automatically get the information.

**You 👩‍🔧**: Nice! In the next step, I’ll help you one step further and insert the received data into Airtable, as you need it.

## 2. Inserting data into Airtable

Before starting to manipulate data from Evil Corp’s data warehouse, it’s helpful to understand how data is structured and why moving it from one source to another is not always straightforward.

<figure><img src="./images/chapter-two/Workflow-with-Airtable-node.png" alt="Workflow with the Airtable node" style="width:100%"><figcaption align = "center"><i>Workflow with the Airtable node</i></figcaption></figure>

If we are going to insert data into Airtable, we first need to set up a table there. To do this:
1. [Create an Airtable account](https://airtable.com/signup).
2. In your Airtable workspace, add a new base from scratch and name it, for example, *beginner course*.

<figure><img src="./images/chapter-two/Create-airtable-base.png" alt="Create an Airtable base" style="width:100%"><figcaption align = "center"><i>Create an Airtable base</i></figcaption></figure>

3. In the beginner course base, you have by default a *Table 1* with four fields: *Name, Notes, Attachment, and Status*.  
These fields are not relevant for us, since they are not in our orders data set. This brings us to the next point: the names of the fields in Airtable have to match the names of the columns in the node result.  
	- Replace the four default table fields with the five column names from the data set. 
	- Also, rename the table from *Table 1* to *orders*, to make it easier to identify. 

Now your table should look like this:

<figure><img src="./images/chapter-two/Orders-table.png" alt="Orders table in Airtable" style="width:100%"><figcaption align = "center"><i>Orders table in Airtable</i></figcaption></figure>

Now that the table is prepared, let’s return to the workflow in the Editor UI. 

Add an ***Airtable node*** connected to the HTTP Request node. In the *Airtable node* window, configure the following parameters:
- *Airtable API:* 
	- *Name:* the name of your credentials (e.g. airtable_api)
	- *API Key:* your API key  
Adding credentials for Airtable is similar to the HTTP Request node you configured in the previous chapter. However, the process of obtaining an API key for Airtable (and other apps/services) is different.
- *Operation:* Append  
This operation will append the new data to the table.
- *Base ID:* the ID of the beginner_course base.  
To get the base Base ID, go to [Airtable's API page](https://airtable.com/api) and click on the base you want to use. The Base ID will be listed in the introduction.
- *Table:* orders

Now execute the *Airtable node* and you should get the following result:

<figure><img src="./images/chapter-two/Airtable-node.png" alt="Airtable node results" style="width:100%"><figcaption align = "center"><i>Airtable node results</i></figcaption></figure>


All 30 data records will now appear in the orders table:

<figure><img src="./images/chapter-two/Airtable-records.png" alt="Imported records in the orders table" style="width:100%"><figcaption align = "center"><i>Imported records in the orders table</i></figcaption></figure>

----
**Nathan 🙋**: Wow, this automation is really useful! But this inserts all collected data into Airtable. Remember that I actually need to insert only processing orders in the table and calculate only the price of booked orders?

**You 👩‍🔧**: Sure, no problem. I'll filter the orders in the next step.

## 3. Filtering orders

To insert only processing orders into Airtable, we need to filter our data by *orderStatus*. Basically, we want to tell the program that _if_ the *orderStatus* is processing, _then_ insert all records with this status into Airtable; _else_, i.e. if the *orderStatus* is not *processing*, calculate the sum of all orders with the other *orderStatus (booked)*.

This if-then-else command is conditional logic. In n8n workflows, conditional logic can be implemented with the [***IF node***](../../nodes/nodes-library/core-nodes/If/README.md), which splits a workflow conditionally based on comparison operations.

::: tip 💡 IF vs Switch
If you need to filter data on more than two conditional routes that are possible with the *IF node* (true and false), use the [*Switch node*](../../nodes/nodes-library/core-nodes/Switch/README.md). The *Switch node* is similar to the *IF node*, but supports up to four conditional routes.
:::

Back to your workflow, remove the connection between the *HTTP Request node* and the *Airtable node*. Add an *IF node* connected to the *HTTP Request node*.

In the *IF node* window, click on *Add Condition* > *string* and configure the parameters:
::: v-pre
- *Value 1*: Current Node > Input Data > JSON > orderStatus → `{{$json["orderStatus"]}}` <br>
To select this value, click on the wheel icon “Add Expression” on the right side of the Value 1 field. 

::: tip 📖 Expressions
An [expression](../../reference/glossary.md#Expression) is a string of characters and symbols in a programming language that represents a value depending upon its input. In n8n workflows, you can use expressions in a node to refer to another node for input data. In our example, the IF node references the data output by the HTTP Request node.
:::

<figure><img src="./images/chapter-two/If-node-expression-editor.png" alt="Expression Editor in the IF node" style="width:100%"><figcaption align = "center"><i>Expression Editor in the IF node</i></figcaption></figure>

- *Operation:* equal
- *Value 2:* processing

:::warning ⚠️ Data Type
Make sure to select the correct data type (boolean, data & time, number, or string) of the referenced data in *Add Condition*.
:::

Now execute the IF node and have a look at the resulted data, which should look like this:

<figure><img src="./images/chapter-two/If-node.png" alt="IF node" style="width:100%"><figcaption align = "center"><i>IF node</i></figcaption></figure>

Next, we want to insert this data into Airtable. You already know how to do this from the previous chapter, where we inserted all data into the *orders* table.

At this stage, your workflow would look like this:


<figure><img src="./images/chapter-two/Workflow-with-If-node.png" alt="Workflow with the IF node" style="width:100%"><figcaption align = "center"><i>Workflow with the IF node</i></figcaption></figure>

But Nathan doesn’t need all the information about the processing orders in Airtable. Sure, he could insert all the five fields “just in case”, but this is not good practice. Inserting more data requires more computational power, the data transfer is slower / takes longer, and takes up more storage resources in your table.

In this particular case, 14 records with 5 features might not seem like a lot to make a significant difference, but if you consider a business with thousands of records and tens of features, things add up and even one extra column can affect performance.

Nathan’s interest in storing processing orders is to have an overview of what employee is responsible for each open order, identified by their id. This means that he needs only the records for employeeName and orderId in Airtable. You’ll learn how to do this in the next lesson.

## 4. Setting values for processing orders
The next step in Nathan’s workflow is to insert the *employeeName* and orderId of all *processing* orders into Airtable.

For this, you need to use the [***Set node***](../../nodes/nodes-library/core-nodes/Set/README.md), which allows you to select and set the data you want to be transferred from one app/service to another. 

::: tip 📖 Set node
The *Set node* can set completely new data as well as overwrite data that already exists. This node is crucial in workflows which expect incoming data from previous nodes, such as when inserting values into spreadsheets or databases.
:::

In your workflow, add a new *Set node* between the *IF node* and the *Airtable node*. In the Set node window, you need to add two values, similarly to the *IF node*. Select:

::: v-pre
- *Add Value > Number:*
  - *Name:* orderId
  - *Value:* `{{$json["orderId"]}}`
    *Current Node > Input Data > JSON > orderID*
- *Add Value > String:*
  - *Name:* employeeName
  - *Value:* `{{$json["employeeName"]}}`
    *Current Node > Input Data > JSON > orderID*
:::

After setting the two values, click on *Execute Node* and you should the following results:

<figure><img src="./images/chapter-two/Set-node.png" alt="Set node" style="width:100%"><figcaption align = "center"><i>Set node</i></figcaption></figure>

Next, we need to insert these values into Airtable. Go to your Airtable and add a new table called *processingOrders* with two columns named *orderId* and *employeeName*, just like you learned in the lesson [Inserting data into Airtable](#inserting-data-into-airtable).

Once that’s done, execute the *Airtable node* in the workflow and you should see the records inserted in the table.

We are getting closer and closer to fulfilling Nathan’s workflow! At this stage, it looks like this:

<figure><img src="./images/chapter-two/Workflow-with-set-node.png" alt="Workflow with the Set node" style="width:100%"><figcaption align = "center"><i>Workflow with the Set node</i></figcaption></figure>

In the next lesson, we’ll continue on the false branch and calculate the value of booked orders.

## 5. Calculating booked orders

The next step in Nathan’s workflow is to calculate two values from the booked orders:
- The total number of booked orders
- The total price of all booked order

To calculate data and add more functionality to your workflows, you can use the ***Function node***, which lets you write custom JavaScript code.

::: warning ⚠️ Function vs Function Item
n8n also provides a **Function Item node**, which should not be confused with the Function node. The Function Item node is used to add custom snippets to JavaScript code that should be executed once for every item that it receives as the input. Learn more about the difference between the Function and Function Item nodes [here](../../reference/function-nodes.md).
:::

Before going into the setup of the Function node, you should first learn the [data structure](../../reference/data/data-structure.md) of n8n. This is important if you want to:
- create your own node
- write custom expressions
- use the Function or Function Item node
- you want to get the most out of n8n

In n8n, the data that is passed between nodes is an array of objects, with the following structure:
```json
[
    {
   	 // Each item has to contain a "json" property. But it can be an empty object like {}.
   	 // Any kind of JSON data is allowed. So arrays and the data being deeply nested is fine.
   	 json: { // The actual data n8n operates on (required)
   		 // This data is only an example it could be any kind of JSON data
   		 jsonKeyName: 'keyValue',
   		 anotherJsonKey: {
   			 lowerLevelJsonKey: 1
   		 }
   	 },
   	 // Binary data of item. The most items in n8n do not contain any (optional)
   	 binary: {
   		 // The key-name "binaryKeyName" is only an example. Any kind of key-name is possible.
   		 binaryKeyName: {
   			 data: '....', // Base64 encoded binary data (required)
   			 mimeType: 'image/png', // Optional but should be set if possible (optional)
   			 fileExtension: 'png', // Optional but should be set if possible (optional)
   			 fileName: 'example.png', // Optional but should be set if possible (optional)
   		 }
   	 }
    },
    ...
]
```
Now let’s see how to implement this.

In your workflow, add a *Function node* connected to the false branch of the *IF node*. In the *Function node* window, paste the following code in the JavaScript Code box:

```javascript
let totalBooked = items.length;
let bookedSum = 0;

for(let i=0; i < items.length; i++) {
  bookedSum = bookedSum + items[i].json.orderPrice;
}
return [{json:{totalBooked, bookedSum}}]

```

Notice the format in which we return the results of the calculation:
`return [{json:{totalBooked, bookedSum}}]`

::: warning ⚠️ Data structure error
If you don’t use the correct data structure, you will get an error message: `Error: Always an Array of items has to be returned!`
:::

Now execute the node and you should see the following results:

<figure><img src="./images/chapter-two/Function-node.png" alt="Function node" style="width:100%"><figcaption align = "center"><i>Function node</i></figcaption></figure>


## 6. Notifying the team

Now that you have a calculated summary of the booked orders, you need to notify Nathan’s team in their Discord channel. n8n has a ***Discord node*** that allows you to send messages.

::: tip 💡 Communication nodes
You can replace the *Discord node* with another communication app. n8n also has nodes for [*Slack*](https://docs.n8n.io/nodes/n8n-nodes-base.slack/) and [*Mattermost*](https://docs.n8n.io/nodes/n8n-nodes-base.mattermost/).
:::

In your workflow, add a *Discord node* connected to the *Function node*. In the *Discord node* window, configure the parameters:
::: v-pre
- *Webhook URL:* [https://discord.com/api/webhooks/862290560479526932/qmSLXOr0RWmP9i7OSPJ-p08mFZbe4CBkxxg8IjUS0Mixxi-VjeLXONY8ZorIqjgILT0F](https://discord.com/api/webhooks/862290560479526932/qmSLXOr0RWmP9i7OSPJ-p08mFZbe4CBkxxg8IjUS0Mixxi-VjeLXONY8ZorIqjgILT0F)
- *Text (Expression):* This week we have {{$json["bookedOrders"]}} booked orders.
:::

<figure><img src="./images/chapter-two/Discord-node.png" alt="Discord node expression" style="width:100%"><figcaption align = "center"><i>Discord node expression</i></figcaption></figure>

Now execute the *Discord node* and if all works well, you should get a message in Discord:

<figure><img src="./images/chapter-two/Discord-output.png" alt="Discord message" style="width:100%"><figcaption align = "center"><i>Discord message</i></figcaption></figure>

----
Amazing! Think of how much time Nathan can save up thanks to this workflow! There’s only one small step left to make it even more effective – scheduling the workflow to run every week. You’ll learn how to do this in the next lesson.

## 7. Scheduling the workflow

The workflow you’ve built so far executes only when you click on _Execute Workflow_. But Nathan needs it to run automatically every Monday morning. You can do this with the ***Cron node***, which allows you to schedule workflows to run periodically at fixed dates, times, or intervals.

In your workflow, replace the *Start node* with the *Cron node* and configure its parameters:
* _Mode:_ Every Week
* _Hour:_ 9
* _Minute:_ 0
* _Weekday:_ Monday

<figure><img src="./images/chapter-two/Cron-node.png" alt="Cron node" style="width:100%"><figcaption align = "center"><i>Cron node</i></figcaption></figure>

----
That was it for the workflow - you've added and configured all necessary nodes! Now every time you click on Execute Workflow, all nodes will be executed, getting and calculating the sales data for Nathan's team. In the next lesson, you will learn how to activate your workflow, so that it runs automatically every week, and how to interpret the execution log.

## 8. Activating and examining the workflow

Activating a workflow means that it will run automatically every time a trigger node receives input or meets a condition. By default, all the newly created workflows are deactivated.

To activate your workflow, toggle the *Active* button on the top right corner of the Editor UI. Nathan’s workflow will now be executed automatically every Monday at 9 am.

<figure><img src="./images/chapter-two/Activated-workflow.png" alt="Activated workflow" style="width:100%"><figcaption align = "center"><i>Activated workflow</i></figcaption></figure>

**Workflow Executions**

An execution represents a completed run of a workflow, from the first to the last node. n8n logs workflow executions, allowing you to see if the workflow was completed successfully or not. The execution log is really useful for debugging your workflow, seeing at what stage it runs into issues.

To see the execution log, click on the icon with three lines in the left panel, which will open the *Workflow Executions* window.

<figure><img src="./images/chapter-two/Execution-list.png" alt="Workflow Execution List" style="width:100%"><figcaption align = "center"><i>Workflow Execution List</i></figcaption></figure>

::: tip 💡 Workflow execution status
In the *Workflow Executions* window, you can filter the displayed executions by workflow and by status (*All*, *Error*, *Running*, or *Success*).
:::

Below, you get a table with information about:

* _Started At / ID:_ the date and time when the workflow started, followed by the ID of this workflow execution
* _Name:_ the name of the workflow
* _Status:_ the status of the workflow (Error, Running, or Success)
* _Mode:_ how the workflow was triggered (trigger or webhook)
* _Running Time:_ the duration it took the workflow to execute


**Workflow Settings**

If you need to customize your workflows and executions or overwrite some of the global default settings, you can do this in *Workflow Settings*. To access them, click on *Workflow Settings* under the *Workflows* section in the left panel.

<figure><img src="./images/chapter-two/Workflow-setting.png" alt="Workflow Setting" style="width:100%"><figcaption align = "center"><i>Workflow Setting</i></figcaption></figure>

In the *Workflow Settings* window, you can configure six settings:

* _[Error Workflow](../../reference/workflow.md#error-workflows):_ A workflow to run in case the execution of the current workflow fails.
* _Timezone:_ The timezone to use in the current workflow. If not set, the global Timezone (by default "New York") is used. This setting is particularly important for the Cron node, as you want to make sure that the workflow gets executed at the right time.
* _Save Data Error Execution:_ If the Execution data of the workflow should be saved when it fails.
* _Save Data Success Execution:_ If the Execution data of the workflow should be saved when it succeeds.
* _Save Manual Executions:_ If executions started from the Editor UI should be saved.
* _Save Execution Progress:_ If the execution data of each node should be saved. If Yes, you can resume the workflow from where it stopped in case of an error, though keep in mind that this might make the execution slower.

----
Now you’ve learned the most important concepts about workflows! In the next lesson, you’ll learn how you can save and share your workflows so that others can benefit from your automation ideas as well.
