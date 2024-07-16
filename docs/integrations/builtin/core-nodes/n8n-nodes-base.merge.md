---
#https://www.notion.so/n8n/Frontmatter-432c2b8dff1f43d4b1c8d20075510fe4
title: Merge
description: Documentation for the Merge node in n8n, a workflow automation platform. Includes guidance on usage, and links to examples.
contentType: integration
priority: critical
---

# Merge

Use the Merge node to combine data from two streams, once data of both streams is available.

/// note | Major changes in 0.194.0
This node was overhauled in n8n 0.194.0. This document reflects the latest version of the node. If you're using an older version of n8n, you can find the previous version of this document [here](https://github.com/n8n-io/n8n-docs/blob/4ff688642cc9ee7ca7d00987847bf4e4515da59d/docs/integrations/builtin/core-nodes/n8n-nodes-base.merge.md){:target=_blank .external-link}.
///

## Merge mode

You can specify how the Merge node should combine data from different branches. The following options are available:

### Append

Keep data from both inputs. The output contains items from Input 1, followed by all items from Input 2.

![Diagram](/_images/integrations/builtin/core-nodes/merge/append-diagram.png)

### Combine

Combine data from both inputs. Choose a **Combination Mode** to control how n8n merges the data.

#### Merge by fields

Compare items by field values. Enter the fields you want to compare in **Fields to Match**.

n8n's default behavior is to keep matching items. You can change this using the **Output Type** setting:

* **Keep Matches**: Merge items that match. This is like an inner join.
* **Keep Non-Matches**: Merge items that don't match.
* **Keep Everything**: Merge items together that do match and include items that don't match. This is like an outer join.
* **Enrich Input 1**: keep all data from Input 1, and add matching data from Input 2. This is like a left join.
* **Enrich Input 2**: keep all data from Input 2, and add matching data from Input 1. This is like a right join.

![Diagram](/_images/integrations/builtin/core-nodes/merge/merge-by-field-diagram.png)


##### Field value clashes

--8<-- "_snippets/integrations/builtin/core-nodes/merge/field-value-clash.md"

##### Multiple matches

Matching by field can generate multiple matches if the inputs contain duplicate data. To handle this, select **Add Option > Multiple Matches**. Then choose:

* **Include All Matches**: Output multiple items if there are multiple matches, one for each match.
* **Include First Match Only**: Keep the first item per match and discard the remaining multiple matches.


#### Merge by position

Combine items based on their order. The item at index 0 in Input 1 merges with the item at index 0 in Input 2, and so on.

![Diagram](/_images/integrations/builtin/core-nodes/merge/merge-by-position-diagram.png)

##### Inputs with different numbers of items

If there are more items in one input than the other, the default behavior is to leave out the items without a match. Choose **Add Option** > **Include Any Unpaired Items** to keep the unmatched items.

##### Field value clashes

--8<-- "_snippets/integrations/builtin/core-nodes/merge/field-value-clash.md"

#### Multiplex

Output all possible item combinations, while merging fields with the same name.

![Diagram](/_images/integrations/builtin/core-nodes/merge/multiplex-diagram.png)

##### Field value clashes

--8<-- "_snippets/integrations/builtin/core-nodes/merge/field-value-clash.md"

#### Options

When combining branches, you can set **Options**:

For all modes:

* **Clash handling**: choose how to merge when branches clash, or when there are sub-fields.
* **Fuzzy compare**: whether to tolerate type differences when comparing fields (enabled), or not (disabled, default). For example, when you enable this, n8n treats `"3"` and `3` as the same.

When merging by field:

* **Disable dot notation**: this prevents accessing child fields using `parent.child` in the field name.
* **Multiple matches**: choose how n8n handles multiple matches when comparing branches.

When merging by position:

**Include Any Unpaired Items**: choose whether to keep or discard unpaired items.

### Choose branch

Choose which input to keep. This option always waits until the data from both inputs is available. You can choose to **Output**:

* The **Input 1 Data**
* The **Input 2 Data**
* **A Single, Empty Item**

The node outputs the data from the chosen input, without changing it.

## Templates and examples

<!-- see https://www.notion.so/n8n/Pull-in-templates-for-the-integrations-pages-37c716837b804d30a33b47475f6e3780 -->
[[ templatesWidget(title, 'merge') ]]

## Merging branches with uneven numbers of items

The items passed into Input 1 of the Merge node will take precedence. For example, if the Merge node receives five items in Input 1 and 10 items in Input 2, it only processes five items. The remaining five items from Input 2 aren't processed.

## Branch execution with If and Merge nodes

--8<-- "_snippets/integrations/builtin/core-nodes/merge/if-merge-branch-execution.md"


## Try it out: A step by step example

Create a workflow with some example input data to try out the Merge node.

### Set up sample data using the Code nodes

1. Add a Code node to the canvas and connect it to the Start node.
2. Paste the following JavaScript code snippet in the **JavaScript Code** field:
```js
return [
  {
    json: {
      name: 'Stefan',
      language: 'de',
    }
  },
  {
    json: {
      name: 'Jim',
      language: 'en',
    }
  },
  {
    json: {
      name: 'Hans',
      language: 'de',
    }
  }
];
```
3. Add a second Code node, and connect it to the Start node.
4. Paste the following JavaScript code snippet in the **JavaScript Code** field:
```js
return [
	  {
    json: {
      greeting: 'Hello',
      language: 'en',
    }
  },
  {
    json: {
      greeting: 'Hallo',
      language: 'de',
    }
  }
];
```

### Try out different merge modes

Add the Merge node. Connect the first Code node to **Input 1**, and the second Code node to **Input 2**. Run the workflow to load data into the Merge node.

The final workflow should look like the following image.

![Merge workflow with two Code nodes](/_images/integrations/builtin/core-nodes/merge/workflow.png)

Now try different options in **Mode** to see how it affects the output data.

#### Append

Select **Mode** > **Append**, then select **Test step**.

Output data in table view:

![Append mode output](/_images/integrations/builtin/core-nodes/merge/append-mode.png)


#### Merge by fields

You can merge these two data inputs so that each person gets the correct greeting for their language.

1. Select **Mode** > **Merge By Fields**.
2. In both **Input 1 Field** and **Input 2 Field**, enter `language`. This tells n8n to combine the data by matching the values in the `language` field in each data set.
3. Select **Test step**.

Output in table view:

![Merge by Fields mode output](/_images/integrations/builtin/core-nodes/merge/merge-by-fields-mode.png)


#### Merge by position

Select **Mode** > **Merge By Position**, then select **Test step**.

Default output in table view:

![Merge by Position mode output](/_images/integrations/builtin/core-nodes/merge/merge-by-position-mode-default.png)


##### Keep unpaired items

If you want to keep all items, select **Add Option** > **Include Any Unpaired Items**, then enable **Include Any Unpaired Items**.

Output with unpaired items in table view:

![Merge by Position mode with unpaired items output](/_images/integrations/builtin/core-nodes/merge/merge-by-position-include-unpaired.png)


#### Multiplex

Select **Mode** > **Multiplex**, then select **Test step**.

Output in table view:

![Merge by Multiplex mode output](/_images/integrations/builtin/core-nodes/merge/multiplex-mode.png)


## Try it out: Load a workflow

n8n provides an example workflow that demonstrates key Merge node concepts.

Go to [Joining different datasets](https://n8n.io/workflows/1747-joining-different-datasets/){:target=_blank .external-link} and select **Use workflow** to copy the example workflow. You can then paste it into your n8n instance.

