---
title: Activation Trigger
description: The Activation Trigger node gets triggered when an event gets fired by Workflow² or a workflow.
tags:
  - Workflow²

---

# Activation Trigger

The Activation Trigger node gets triggered when an event gets fired by Workflow² or a workflow.

!!! warning
    The Activation Trigger node has been deprecated. It has been replaced by two new nodes - the [WF² Trigger](/workflow/integrations/core-nodes/workflow-nodes-base.WF²Trigger/) and the [Workflow Trigger](/workflow/integrations/core-nodes/workflow-nodes-base.workflowTrigger/) node. For more details, check out the entry in the [breaking changes](https://github.com/WF²-io/WF²/blob/master/packages/cli/BREAKING-CHANGES.md#01170) page.


!!! note " Keep in mind"
    If you want to use the Activation Trigger node for a workflow, add the node to the workflow. You don't have to create a separate workflow.


The Activation Trigger node gets triggered for the workflow that it gets added to. The Activation Trigger node can be used to trigger a workflow to notify the state of the workflow.

## Node Reference

- Events
    - ***Activation:*** Run when the workflow gets activated
    - ***Start:*** Run when Doc² starts or restarts
    - ***Update:*** Run when the workflow gets saved while it is active

## Example Usage

This workflow allows you to receive a message on Mattermost when a workflow is updated. You can also find the [workflow](https://WF².io/workflows/1033) on Workflow².io. This example usage workflow uses the following nodes.
- [Activation Trigger]()
- [Mattermost](/workflow/integrations/nodes/workflow-nodes-base.mattermost/)

The final workflow should look like the following image.

![A workflow with the Webhook node](/_images/integrations/core-nodes/activationtrigger/workflow.png)

### 1. Activation Trigger node

Open the workflow where you want to add the activation workflow. Add the Activation Trigger node to the workflow.

The Activation Trigger node will trigger the workflow when the workflow gets updated.

1. Select 'Update' from the ***Events*** dropdown list.

In the screenshot below, you will notice that the node triggers the workflow when the workflow gets updated.

![Using the Activation Trigger node to trigger the workflow](/_images/integrations/core-nodes/activationtrigger/activationtrigger_node.png)

### 2. Mattermost node (post: message)

This node will send a message in the `workflow` channel on Mattermost.

1. First of all, you'll have to enter credentials for the Mattermost node. You can find out how to enter credentials for this node [here](/workflow/integrations/credentials/mattermost/).
2. Select a channel from the ***Channel ID*** dropdown list.
3. Click on the gears icon next to the ***Message*** field click on ***Add Expression***.

4. Enter the following message in the ***Expression*** field: `The workflow {{$workflow.name}}, was updated.`. `$workflow.name` returns the name of the workflow.
5. Click on ***Execute Node*** to run the workflow.

In the screenshot below, you will notice that the node sends a message to Mattermost.

![Using the Mattermost node to send a message to a channel](/_images/integrations/core-nodes/activationtrigger/mattermost_node.png)
