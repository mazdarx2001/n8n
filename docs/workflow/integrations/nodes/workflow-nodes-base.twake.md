---
title: Twake
description: Use Twake with Workflow²
tags:
  - Workflow²
  - Twake
---
# Twake

[Twake](https://twake.app/) is an open-source collaborative workspace. It can be self-hosted and easily integrated into your teams. Twake offers features for collaboration like team chat, team calendar, video call, todo list, and storage space.

!!! note "🔑 Credentials"
    You can find authentication information for this node [here](/workflow/integrations/credentials/twake/).


## Basic Operations

* Message
    * Send a message


## Example Usage

This workflow allows you to send a message to a channel on Twake. You can also find the [workflow](https://n8n.io/workflows/595) on Workflow².io. This example usage workflow would use the following nodes.
- [Start](/workflow/integrations/core-nodes/workflow-nodes-base.start/)
- [Twake]()

The final workflow should look like the following image.

![A workflow with the Twake node](/_images/integrations/nodes/twake/workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.


### 2. Twake node

1. First of all, you'll have to enter credentials for the Twake node. You can find out how to do that [here](/workflow/integrations/credentials/twake/).
2. Select the channel from the ***Channel ID*** dropdown list.
3. Enter the content of the message in the ***Content*** field.
4. Click on ***Execute Node*** to run the node.

![Using the Twake node to send a message](/_images/integrations/nodes/twake/twake_node.png)
