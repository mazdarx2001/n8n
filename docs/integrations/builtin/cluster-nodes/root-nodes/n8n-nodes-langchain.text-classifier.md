---
#https://www.notion.so/n8n/Frontmatter-432c2b8dff1f43d4b1c8d20075510fe4
title: Text Classifier
description: Documentation for the Text Classifier node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
contentType: integration
---

# Text Classifier

Use the Text Classifier node to classify (categorize) incoming data. Using the
categories provided in the parameters (see below), each item is passed to the
model to determine its category.

On this page, you'll find the node parameters for the Text Classifier node,
and links to more resources.

## Node parameters

**Input Prompt** defines the input to classify. This is usually an expression
that references a field from the input items. For example, this could be 
`{{ $json.chatInput }}` if the input is a chat trigger. By default it
references the `text` field.

**Categories**: Add the categories that you want to classify your input as.
Categories have a name and a description. Use the description to tell the
model what the category means. This is important if the meaning isn't obvious.
You can add as many categories as you like.

## Node options

* **Allow Multiple Classes To Be True**: You can configure the classifier to
  always output a single class per item, or allow the model to select multiple
  classes.

* **When No Clear Match**: This option allows you to define what happens if
  the model can't find a good match for an item. There are two options:

	- **Discard Item** (the default): If none of the categories are detected,
	  the item is dropped.

	- **Output on Extra, 'Other' Branch**: Creates a separate output branch
	  called 'Other', for when none of the categories are detected.

* **System Prompt Template**: This option allows you to change the system prompt that's used for the classification. It uses the `{categories}` placeholder for the categories.


## Related resources

--8<-- "_snippets/integrations/builtin/cluster-nodes/langchain-overview-link.md"
--8<-- "_glossary/ai-glossary.md"
