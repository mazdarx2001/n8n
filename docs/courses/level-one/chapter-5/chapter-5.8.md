---
contentType: tutorial
---

# 8. Activating and Examining the Workflow

In this step of the workflow you will learn how to activate your workflow and change the default workflow settings.

Activating a workflow means that it will run automatically every time a trigger node receives input or meets a condition. By default, all newly created workflows are deactivated.

To activate your workflow toggle the *Active* button on the top right corner of the Editor UI. Nathan's workflow will now be executed automatically every Monday at 9 AM.

<figure><img src="/_images/courses/level-one/chapter-five/l1-c5-5-8-activated-workflow.png" alt="Activated workflow" style="width:100%"><figcaption align = "center"><i>Activated workflow</i></figcaption></figure>

**Workflow Executions**

An execution represents a completed run of a workflow, from the first to the last node. n8n logs workflow executions, allowing you to see if the workflow was completed successfully or not. The execution log is useful for debugging your workflow and seeing at what stage it runs into issues.

To see the execution log, in your Editor UI click on *Executions* in the left panel. This will open the *Workflow Executions* window.

<figure><img src="/_images/courses/level-one/chapter-five/l1-c5-5-8-execution-list.png" alt="Workflow Execution List" style="width:100%"><figcaption align = "center"><i>Workflow Execution List</i></figcaption></figure>

The *Workflow Executions* window displays a table with the following information:

* _Name:_  The name of the workflow
* _Started At:_ The date and time when the workflow started
* _Status / Running time:_ The status of the workflow (Running, Succeeded or Error) / The duration it took the workflow to execute
* _Execution ID:_ The ID of this workflow execution

/// note | Workflow execution status
In the **Workflow Executions** window you can filter the displayed executions by workflow and by status (**All**, **Error**, **Running**, or **Success**).
The information displayed here depends on what workflows and executions you set up in *Workflow Settings* to be saved.
///


**Workflow Settings**

You can customize your workflows and executions, or overwrite some of the global default settings in *Workflow Settings*. These settings are located in the top right of the Editor UI, and can be accessed by clicking on the 3 dots and then settings.

<figure><img src="/_images/courses/level-one/chapter-five/l1-c5-5-8-workflow-settings.png" alt="Workflow Settings" style="width:100%"><figcaption align = "center"><i>Workflow Settings</i></figcaption></figure>

In the *Workflow Settings* window you can configure the following settings:

* _[Error Workflow](/flow-logic/error-handling/){:target="_blank" .external}:_ A workflow to run in case the execution of the current workflow fails.
* _This workflow can be called by:_ Workflows that are allowed to call this workflow using the Execute Workflow node
* _Timezone:_ The timezone to use in the current workflow. If not set, the global Timezone (by default "New York") is used. This setting is particularly important for the Schedule Trigger node, as you want to make sure that the workflow gets executed at the right time.
* _Save failed production executions:_ If the Execution data of the workflow should be saved when it fails.
* _Save successful production executions:_ If the Execution data of the workflow should be saved when it succeeds.
* _Save manual executions:_ If executions started from the Editor UI should be saved.
* _Save execution progress:_ If the execution data of each node should be saved. If Yes, you can resume the workflow from where it stopped in case of an error, though keep in mind that this might make the execution slower.
* _Timeout Workflow:_ Whether to cancel a workflow execution after a specific period of time


## What's next?

**You 👩‍🔧**: That was it! Now you have a 7-node workflow that will run automatically every Monday morning. You don't have to worry about remembering to wrangle the data. Instead, you can start your week with more meaningful or exciting work.

**Nathan 🙋**: This workflow is incredibly helpful, thank you! Now, what's next for you?

**You 👩‍🔧**: I'd like to build more workflows, share them with others, and use some workflows built by other people.
