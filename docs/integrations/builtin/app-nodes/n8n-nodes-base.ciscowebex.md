---
title: Webex by Cisco
description: Documentation for the Webex by Cisco node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

# Webex by Cisco

The Webex by Cisco node allows you to automate work in Webex, and integrate Webex with other applications. n8n has built-in support for a wide range of Webex features, including creating, getting, updating, and deleting meetings and messages.

On this page, you'll find a list of operations the Webex node supports and links to more resources.

!!! note "Credentials"
    Refer to [Webex credentials](/integrations/builtin/credentials/ciscowebex/) for guidance on setting up authentication. 

!!! note "Examples and Templates"
    For usage examples and templates to help you get started, take a look at n8n's [Webex integrations](https://n8n.io/integrations/webex-by-cisco/){:target=_blank .external-link} list.


!!! note "Examples and Templates"
  For usage examples and templates to help you get started, take a look at n8n's [Webex integrations](https://n8n.io/integrations/webex-by-cisco/){:target=_blank .external-link} list.

## Basic operations

* Meeting
    * Create
    * Delete
    * Get
    * Get All
    * Update
* Message
    * Create
    * Delete
    * Get
    * Get All
    * Update

## Example usage

This workflow allows you to create a new meeting. This example usage workflow uses the following node:

- [Webex by Cisco]()

The final workflow should look like the following image.

![A workflow with the Webex by Cisco node](/_images/integrations/builtin/app-nodes/ciscowebex/workflow.png)

### 1. Webex by Cisco node

1. First enter your credentials for node. You can find out how to do that [here](/integrations/builtin/credentials/ciscowebex/).
2. Select 'Meeting' from the *Resource* dropdown list.
3. Select 'Create' from the *Operation* dropdown list.
4. Enter a *Title* for your new meeting.
5. Select the *Start* and *End* times for the meeting.
6. Optionally, use the *Additional Fields* menu to add further meeting details, for example an agenda, set the invitees, or a meeting recurrence.
7. Click on *Execute Node* to run the workflow.

![The Webex by Cisco node](/_images/integrations/builtin/app-nodes/ciscowebex/webex_node.png)

