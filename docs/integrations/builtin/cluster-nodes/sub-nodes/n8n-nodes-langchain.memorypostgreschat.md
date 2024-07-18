---
title: Postgres Chat Memory
description: Documentation for the Postgres Chat Memory node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

# Postgres Chat Memory

Use the Postgres Chat Memory node to use Postgres as a memory server for storing chat history.

On this page, you'll find a list of operations the Postgres Chat Memory node supports, and links to more resources.

/// note | Credentials
You can find authentication information for this node [here](/integrations/builtin/credentials/postgres/).
///

--8<-- "_snippets/integrations/builtin/cluster-nodes/sub-node-expression-resolution.md"

## Node parameters

* **Session Key**: the key to use to store the memory in the workflow data.
* **Table Name**: the name of the table to store the chat history in. The system will create the table if doesn't exist.

## Related resources

Refer to [LangChain's Postgres Chat Message History documentation](https://js.langchain.com/docs/modules/memory/integrations/postgres){:target=_blank .external-link} for more information about the service.

--8<-- "_snippets/integrations/builtin/cluster-nodes/langchain-overview-link.md"

## Single memory instance

[[% include "_includes/integrations/cluster-nodes/memory-shared.html" %]]

--8<-- "_glossary/ai-glossary.md"
