# Navigating the Editor UI

> In this lesson, you will learn to navigate the Editor UI. We will walk through the canvas and show you what each icon means and where to find things. Don’t worry if you don’t understand some of the concepts that are mentioned, we will explain them in detail as we build the workflow.

[[toc]]

## Getting started

First of all, you need to set up n8n. There are different ways to [get started with n8n](https://docs.n8n.io/getting-started/quickstart.html#sign-up-on-n8n-cloud): you can [install it locally with npm](https://docs.n8n.io/getting-started/quickstart.html#install-with-npm), run it with Docker, or sign up on [n8n.cloud](http://n8n.cloud). The option you choose depends on your preference and technical requirements.

**In this course, we will use an n8n.cloud instance with the n8n version 0.127.0.**

Once you have n8n installed or set up, open the Editor UI in a browser window, which looks like this:

<figure><img src="./images/chapter-one/Editor-UI.png" alt="Editor UI" style="width:100%"><figcaption align = "center"><i>Editor UI</i></figcaption></figure>

Now that you have the Editor UI open, you'll learn how to navigate it.

## Editor UI settings

The [Editor UI](http://docs.n8n.io/reference/glossary.html#editor-ui) represents the web interface used to create [workflows](http://docs.n8n.io/getting-started/key-components/workflow.html). Think of it as a canvas where the artist in you creates automations. From the Editor UI, you can access all your workflows and credentials, as well as the n8n documentation and forum.

### Left-side panel
Right under the n8n logo in the upper left corner, you will notice a round arrow icon. Click on it to open the left-side menu, which contains the core functionalities and settings for managing workflows.

<figure><img src="./images/chapter-one/Left-side-menu.png" alt="Editor UI left-side menu" style="width:30%"><figcaption align = "center"><i>Editor UI left-side menu</i></figcaption></figure>


There are four main sections in the left menu:
- (The *Admin Panel*, if you use n8n.cloud)
- The *Workflows* section includes operations for creating and editing workflows.
- The *Credentials* section includes operations for creating credentials.
- The *Executions* section includes information about your workflow [executions](http://docs.n8n.io/reference/glossary.html#execution), which are complete runs of a workflow from the first to the last node.
- The *Help* section includes resources around n8n product and community.

### Top bar

The top bar of the Editor UI contains four pieces of information:

<figure><img src="./images/chapter-one/Editor-UI-top-bar.png" alt="Editor UI top bar" style="width:100%"><figcaption align = "center"><i>Editor UI top bar</i></figcaption></figure>

- The text that appears in the top left is the *name* of the current workflow.
- Next to it, you have the option to add a *tag*. Tags help you organize your workflows by use case, domain, or whatever is relevant for you.
- In the top right corner of the Editor UI, there is an orange *Save* button that saves the current workflow.
- Next to it, there is a *toggle* button, with which you can activate or deactivate the current workflow.

### Canvas

The *canvas* is the grey grid background in the Editor UI. On the canvas, you there are five buttons and a node with different functionalities:

<figure><img src="./images/chapter-one/Workflow-canvas.png" alt="Workflow canvas" style="width:100%"><figcaption align = "center"><i>Workflow canvas</i></figcaption></figure>

- In the left corner of the canvas, there are three small icons. By clicking on them, you can zoom in (**+**) or out (**-**) of the canvas and reset (**←**) the canvas to the original resolution.
- At the bottom center of the canvas there is an orange button called *Execute Workflow*. When you click on it, it will execute all nodes on the canvas.
- On the top right corner of the canvas there is an orange circle with a *+* sign inside. This button opens the nodes panel and you’ll learn more about nodes in the following chapter.
- In the center of the canvas, there is a square with a green play icon inside. This is the *Start node*. You will learn more about nodes in the [next section](#nodes).

Don’t worry about workflow execution and activation for now, we will explain these concepts in the lesson Running the workflow.

## Nodes

The [*Start node*](https://docs.n8n.io/nodes/n8n-nodes-base.start) is the default starting point in any workflow. Every time you create a new workflow, a *Start node* will be included by default.

<figure><img src="./images/chapter-one/Start-node.png" alt="Start node" style="width:50%"><figcaption align = "center"><i>Start node</i></figcaption></figure>

You can think of nodes as building blocks that serve different functions but put together, they make up a functioning machinery – an automated workflow.

::: tip 📖 Node
Technically, a [node](http://docs.n8n.io/reference/glossary.html#node) is an entry point for retrieving data, a function to process data, or an exit point for sending data. The functions can be pretty much anything, like data processing or conditional filtering.
:::

Based on their function, nodes can be classified into three types:

- **Regular Nodes** add, remove, and edit data, as well as request and send external data.
- **Trigger Nodes** start a workflow and supply the initial data.
- **Core Nodes** are those that do not represent an app or a service, instead they serve general functions, like scheduling workflows or adding JavaScript functions. Core Nodes can function as regular nodes or as triggers.

You’ve probably figured out already that the *Start node* is a Core Trigger node. Apart from it, there are over 200 other Regular and Trigger nodes for various functions, apps, and services.

### Finding nodes

You can find all available nodes in the nodes panel on the right side of the Editor UI. There are three ways in which you can open the nodes panel:

- Click on the *+* icon in the top right corner of the canvas.
- Click on the grey dot on the right side of an existing node on the canvas (the node to which you want to add another one) and pull the connection line to the right.
- Click on the Tab key on your keyboard.

The nodes panel looks like this:

<figure><img src="./images/chapter-one/Nodes-panel.png" alt="Nodes panel" style="width:50%"><figcaption align = "center"><i>Nodes panel</i></figcaption></figure>

In the nodes panel, notice that the nodes are grouped in three tabs: All, Regular, and Trigger. In addition, nodes are also grouped by their functionality domain (like Analytics or Sales). This makes it easier to find the right nodes you need. 

If you want to get a specific node, type in the name of the node, app, or service in the search field and select the respective tab.

### Adding nodes

To add a new node to the Editor UI, simply click on the node you want in the nodes panel. The new node will automatically be connected to the last added node on the canvas.

So, to recapitulate here’s a walkthrough of the Editor UI touching on all the settings you’ve learned in this chapter:

<figure><img src="./images/chapter-one/Editor-UI-walkthrough.gif" alt="Editor UI walkthrough" style="width:100%"><figcaption align = "center"><i>Editor UI walkthrough</i></figcaption></figure>


### Node executions

::: tip 📖 Node execution
A node execution represents a run of that node, to retrieve the specified data.
:::

If the parameters are configured correctly and everything works fine, the requested data will be displayed in the node window in *Table* and *JSON* format. You can switch between these views by selecting the one you want from the *JSON|Table* button at the top of the node window.

::: tip 📖 Table vs JSON views
The *Table* view is the default. It displays the requested data in a table, where the rows are the records and the columns are the available attributes of those records.
:::

<figure><img src="./images/chapter-one/Hacker-news-json.png" alt="Results in JSON view for the Hacker News node" style="width:100%"><figcaption align = "center"><i>Results in JSON view for the Hacker News node</i></figcaption></figure>

The node window displays more information about the node execution:

- In the top left corner of the results window, you’ll notice another piece of information: ***Items**: 10*.  
This field displays the number of items (records) that are returned by the node request. In our case, it’s expected to be 10, since this is the limit we set in the node. But if you don’t set a limit, it’s useful to see how many records are actually returned.
- Next to the *Items* information, notice a small orange *i* icon. If you hover on it, you’ll get two more pieces of information: ***Start Time*** (when the node execution started) and ***Execution Time*** (how long it took for the node to return the results from the moment it started executing).  
*Start Time* and *Execution Time* can provide insights into the performance of each individual node.
- In the bottom right corner right under the node window, there is a reference link to the node’s **documentation**. Check it out if you ever run into troubles or are not sure how to configure the node’s parameters.

### Node buttons

If a node executed successfully, a small green circle with a number inside will appear on top of the node.

<figure><img src="./images/chapter-one/Hacker-news-success.png" alt="Successfully executed workflow" style="width:100%"><figcaption align = "center"><i>Successfully executed workflow</i></figcaption></figure>

If you go ahead and hover on the node, you’ll notice that four other icons appear on top of it:

- Delete the node
- Deactivate/Activate the node
- Duplicate the node
- Execute the node

<figure><img src="./images/chapter-one/Node-buttons.gif" alt="The four node buttons" style="width:100%"><figcaption align = "center"><i>The four node buttons</i></figcaption></figure>


::: warning ⚠️ Start node
The **Start** node cannot be deleted or duplicated. If you have a workflow in which you don’t use the Start node, you can remove the connection, deactivate it, and move it away from the workflow. If you need more than one Start node, you probably need to use other Trigger nodes or create separate workflows.
:::

If you want to edit the parameters of a node, double-click on it and it will open the node window.

::: tip 💡 Moving the canvas
You can move the workflow canvas around in two ways:
- Click **Ctrl + Left Mouse Button** on the canvas and move it around
- Place two fingers on your touchpad and slide

To move a workflow around the canvas, select all nodes (**Ctrl + A**), click on a node, and drag it at a point you want on the canvas.
:::

----
## Summary
In this lesson, you learned how to navigate the Editor UI, what the icons mean, how to access the left-side and node panels, how to add nodes to the canvas and interpret their execution results.

In the next lesson, you will build a mini-workflow to put into practice what you've learned so far. 