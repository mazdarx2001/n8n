---
description: A node is an entry point for retrieving data, a function to process data, or an exit for sending data.
contentType: howto
---

# Nodes

Nodes are the key building blocks of a workflow. They perform a range of actions, including:

* Starting the workflow.
* Fetching and sending data.
* Processing and manipulating data.

n8n provides a collection of built-in nodes, as well as the ability to create your own nodes. Refer to:

* [Built-in integrations](/integrations/builtin/node-types/) to browse the node library.
* [Community nodes](/integrations/community-nodes/installation/) for guidance on finding and installing community-created nodes.
* [Creating nodes](/integrations/creating-nodes/overview/) to start building your own nodes.


## Add a node to your workflow

### Add a node to an empty workflow

1. Select **Add first step**. n8n opens the nodes panel, where you can search or browse trigger nodes.
2. Select the trigger you want to use.

    /// note | Choose the correct app event
	If you select **On App Event**, n8n shows a list of all the supported services. This allows you to browse n8n's integrations and trigger a workflow in response to an event in your chosen service. However, not all integrations have triggers. To see which ones you can use as a trigger, select the node. If a trigger is available, you'll see it at the top of the available operations list.

	For example, this is the trigger for Asana:

	![Screenshot of the Asana node operations list, showing the Recommended section at the top of the list](/_images/workflows/components/nodes/recommended-trigger.png)
	///

### Add a node to an existing workflow

Select the **Add node** <span class="inline-image">![Add node icon](/_images/try-it-out/add-node-small.png)</span> connector. n8n opens the nodes panel, where you can search or browse all nodes.

--8<-- "_snippets/integrations/builtin/node-operations.md"

## Node controls

To view node controls, hover over the node on the canvas:

* **Play** <span class="inline-image">![Run node icon](/_images/common-icons/play-node.png)</span> : run the node.
* **Node context menu** <span class="inline-image">![Node context menu icon](/_images/common-icons/node-context-menu.png)</span>: select node actions. Available actions:
	* Open node
	* Execute node
	* Rename node
	* Deactivate node
	* Pin node
	* Copy node
	* Duplicate node
	* Select all
	* Clear selection
	* Delete node

## Node settings

The node settings allow you to control node behaviors and add node notes.

There are four toggles. When active, they do the following:

* **Always Output Data**: the node returns an empty item even if the node returns no data during execution. Be careful setting this on IF nodes, as it could cause an infinite loop.
* **Execute Once**: the node executes once, with data from the first item it receives. It doesn't process any additional items.
* **Retry On Fail**: when an execution fails, the node reruns until it succeeds. 
* **Continue On Fail**: the workflow continues even if the execution of the node fails. When this happens, the node passes along input data from previous nodes, so if you enable this setting, the workflow design must handle unexpected output data.

You can document your workflow using node notes:

* **Notes**: note to save with the node.
* **Display note in flow**: if active, n8n displays the note in the workflow as a subtitle.
