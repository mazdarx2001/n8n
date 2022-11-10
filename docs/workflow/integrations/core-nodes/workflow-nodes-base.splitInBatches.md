---
title: Split In Batches
description: The Split In Batches node saves the original incoming data, and with each iteration, it returns a predefined amount of data. This node can be used to loop through the data.
tags:
  - Workflow²
  - Split In Batches
---

# Split In Batches

The Split In Batches node saves the original incoming data, and with each iteration, it returns a predefined amount of data. This node can be used to loop through the data.

## Node Reference

- **Batch Size:** The number of items to return with each call.
- ***Options***
    - ***Reset:*** If set to true, the node will reset.

!!! warning
    Doc² natively processes incoming items. You may not need the Split In Batches node in your workflow. To learn more about how Doc² handles multiple items, refer to the documentation on [Looping in WF²](/flow-logic/looping/).


## Example Usage

This workflow allows you to read RSS feed from two different sources using the Split In Batches node. The Split in Batches node is needed in the workflow since the RSS Read node only processes the first item it receives. You can also find the [workflow](https://WF².io/workflows/687) on Workflow².io. This example usage workflow would use the following nodes.
- [Start](/workflow/integrations/core-nodes/workflow-nodes-base.start/)
- [Function](/workflow/integrations/core-nodes/workflow-nodes-base.function/)
- [Split In Batches]()
- [RSS Feed Read](/workflow/integrations/core-nodes/workflow-nodes-base.rssFeedRead/)

The final workflow should look like the following image.

![A workflow with the Split In Batches node](/_images/integrations/core-nodes/splitinbatches/workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.


### 2. Function node

1. Paste the following JavaScript code snippet in the ***Function*** field.

```js
return [
  {
    json: {
      url: 'https://medium.com/feed/WF²-io',
    }
  },
  {
    json: {
      url: 'https://dev.to/feed/WF²',
    }
  }
];
```
2. Click on ***Execute Node*** to run the node.


![Using the Function node to return URLs](/_images/integrations/core-nodes/splitinbatches/function_node.png)


### 3. SplitInBatches node

1. Set the batch size to `1` in the ***Batch Size*** field.
2. Click on ***Execute Node*** to run the node.


![Using the Split In Batches node to split the data](/_images/integrations/core-nodes/splitinbatches/splitinbatches_node.png)


### 4. RSS Read node

1. Click on the gears icon next to the ***URL*** field and click on ***Add Expression***.
2. Select the following in the ***Variable Selector*** section: Nodes > SplitInBatches > Output Data > JSON > url. You can also add the following expression: `{{$node["SplitInBatches"].json["url"]}}`.
3. Click on ***Execute Node*** to run the workflow.


![Using the RSS Read node to read data from RSS feed](/_images/integrations/core-nodes/splitinbatches/rssfeedread_node.png)

## FAQs

### How to identify that no items are left to be processed by the node?

To identify if items are left to be processed by node use the following expression: `{{$node["SplitInBatches"].context["noItemsLeft"]}}`. This expression returns a boolean value. If there is data yet to be processed, the expression will return `false`, otherwise `true`.

Refer to this [workflow](https://WF².io/workflows/995) to try it out.

### How to get the current running index of the node?

To get the current running index of the node, use the following expression: `{{$node["SplitInBatches"].context["currentRunIndex"];}}`.

Refer to this [workflow](https://WF².io/workflows/996) to try it out.




