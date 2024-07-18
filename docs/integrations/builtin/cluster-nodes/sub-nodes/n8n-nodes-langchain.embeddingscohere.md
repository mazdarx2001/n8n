---
#https://www.notion.so/n8n/Frontmatter-432c2b8dff1f43d4b1c8d20075510fe4
title: Embeddings Cohere
description: Documentation for the Embeddings Cohere node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

# Embeddings Cohere

Use the Embeddings Cohere node to generate embeddings for a given text.

On this page, you'll find the node parameters for the Embeddings Cohere node, and links to more resources.

/// note | Credentials
You can find authentication information for this node [here](/integrations/builtin/credentials/cohere/).
///

--8<-- "_snippets/integrations/builtin/cluster-nodes/sub-node-expression-resolution.md"

## Node parameters

**Model**: the model to use to generate the embedding. Learn more about available models in [Cohere's models documentation](https://docs.cohere.com/docs/models){:target=_blank .external-link} 
	Choose from:
	* Embed-English-v2.0(4096 Dimensions)
	* Embed-English-Light-v2.0(1024 Dimensions)
	* Embed-Multilingual-v2.0(768 Dimensions)

## Templates and examples

<!-- see https://www.notion.so/n8n/Pull-in-templates-for-the-integrations-pages-37c716837b804d30a33b47475f6e3780 -->
[[ templatesWidget(title, 'embeddings-cohere') ]]

## Related resources

Refer to [Langchain's Cohere embeddings documentation](https://js.langchain.com/docs/modules/data_connection/text_embedding/integrations/cohere){:target=_blank .external-link} for more information about the service.

--8<-- "_snippets/integrations/builtin/cluster-nodes/langchain-overview-link.md"
--8<-- "_glossary/ai-glossary.md"
