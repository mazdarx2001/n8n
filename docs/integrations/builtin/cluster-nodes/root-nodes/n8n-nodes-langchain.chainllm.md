---
#https://www.notion.so/n8n/Frontmatter-432c2b8dff1f43d4b1c8d20075510fe4
title: Basic LLM Chain
description: Documentation for the Basic LLM Chain node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
priority: critical
---

# Basic LLM Chain

Use the Basic LLM Chain node to set the prompt that the model will use along with setting an optional parser for the response.

On this page, you'll find the node parameters for the Basic LLM Chain node, and links to more resources.

/// note | Examples and templates
For usage examples and templates to help you get started, refer to n8n's [Basic LLM Chain integrations](https://n8n.io/integrations/basic-llm-chain/){:target=_blank .external-link} page.
///	

## Node parameters

### Prompt

This is the prompt that the model uses. For example:

```
Tell me a joke about {{ $json.input }}
```

### Chat Messages

Use this when using a chat model to set a message. n8n ignores these options if you don't connect a chat model.

* AI: provide a response. The model will try to respond in the same way in its messages.
* System: set a system message to accompany the user input. Use this for things like defining tone. For example "Always respond talking like a pirate."
* User: provide a sample user input. Using this with the AI option can help improve the output of the agent. Using both together provides a sample of an input and expected response (the AI message) for the model to follow.

## Templates and examples

<!-- see https://www.notion.so/n8n/Pull-in-templates-for-the-integrations-pages-37c716837b804d30a33b47475f6e3780 -->
[[ templatesWidget(title, 'basic-llm-chain') ]]

## Related resources

Refer to [LangChain's documentation on Basic LLM Chains](https://js.langchain.com/docs/modules/chains/foundational/llm_chain){:target=_blank .external-link} for more information about the service.

--8<-- "_snippets/integrations/builtin/cluster-nodes/langchain-overview-link.md"
--8<-- "_glossary/ai-glossary.md"
