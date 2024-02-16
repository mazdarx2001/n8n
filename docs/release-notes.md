---
title: Release notes
description: Release notes detailing new features and bug fixes for n8n.
tags:
  - release
  - release notes
  - changelog
hide:
  - tags
contentType: reference
---
<!-- vale off -->
# Release notes

New features and bug fixes for n8n.

You can also view the [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} in the GitHub repository.

--8<-- "_snippets/self-hosting/installation/latest-next-version.md"

--8<-- "_snippets/update-n8n.md"

## Semantic versioning in n8n

n8n uses [semantic versioning](https://semver.org/){:target=_blank .external-link}. All version numbers are in the format `MAJOR.MINOR.PATCH`. Version numbers increment as follows:

* MAJOR version when making incompatible changes which can require user action.
* MINOR version when adding functionality in a backward-compatible manner.
* PATCH version when making backward-compatible bug fixes.

## n8n@1.29.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.29.0...n8n@1.29.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-02-16

/// note | Next version
This is the `next` version. n8n recommends using the `latest` version. The `next` version may be unstable. To report issues, use the [forum](https://community.n8n.io/c/questions/12){:target=_blank .external-link}.
///

This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.29.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.28.0...n8n@1.29.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-02-15

This release contains new features, node enhancements, and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### New features

<div class="n8n-new-features" markdown>

#### OpenAI node overhaul

This release includes a new version of the [OpenAI node](/integrations/builtin/app-nodes/n8n-nodes-base.openai/), adding more operations, including support for working with assistants.

</div>

Other highlights:

* Support for AI events in [log streaming](/log-streaming/).
* Added support for workflow tags in the [public API](/api/).

### Contributors

[Bruno Inec](https://github.com/sweenu){:target=_blank .external-link}  
[Jesús Burgers](https://github.com/jburgers-chakray){:target=_blank .external-link}

## n8n@1.27.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.27.2...n8n@1.27.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-02-15

/// note | Latest version
This is the `latest` version. n8n recommends using the `latest` version. The `next` version may be unstable. To report issues, use the [forum](https://community.n8n.io/c/questions/12){:target=_blank .external-link}.
///



This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.28.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.27.2...n8n@1.28.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-02-07



This release contains new features, new nodes, node enhancements and bug fixes.

<div class="n8n-new-features" markdown>

#### New nodes: Azure OpenAI chat model and embeddings 

This release adds two new nodes to work with [Azure OpenAI](https://azure.microsoft.com/en-gb/products/ai-services/openai-service/){:target=_blank .external-link} in your advanced AI workflows:

* [Embeddings Azure OpenAI](/integrations/builtin/cluster-nodes/sub-nodes/n8n-nodes-langchain.embeddingsazureopenai/)
* [Azure OpenAI Chat Model](/integrations/builtin/cluster-nodes/sub-nodes/n8n-nodes-langchain.lmchatazureopenai/)

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Andrea Ascari](https://github.com/ascariandrea){:target=_blank .external-link}

## n8n@1.27.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.27.1...n8n@1.27.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-02-02

This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.27.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.26.0...n8n@1.27.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-01-31

This release contains new features, node enhancements, and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.27.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.26.0...n8n@1.27.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-01-31

/// warning | Breaking change
This release removes `own` mode for self-hosted n8n. You must now use `EXECUTIONS_MODE` and set to either `regular` or `queue`. Refer to [Queue mode](/hosting/scaling/queue-mode/) for information on configuring queue mode.
///

/// note | Skip this release
Please upgrade directly to 1.27.1.
///

This release contains node enhancements and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.26.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.25.1...n8n@1.26.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-01-24

This release contains new features, node enhancements, and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Daniel Schröder](https://github.com/schroedan){:target=_blank .external-link}  
[Nihaal Sangha](https://github.com/nihaals){:target=_blank .external-link}

## n8n@1.25.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.25.0...n8n@1.25.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-01-22

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Nihaal Sangha](https://github.com/nihaals){:target=_blank .external-link}

## n8n@1.25.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.24.1...n8n@1.25.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-01-17

This release contains a new node, feature improvements, and bug fixes.

<div class="n8n-new-features" markdown>

#### New node: Chat Memory Manager

The [Chat Memory Manager](/integrations/builtin/cluster-nodes/sub-nodes/n8n-nodes-langchain.memorymanager/) node replaces the Chat Messages Retriever node. It manages chat message memories within your AI workflows.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.24.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.24.0...n8n@1.24.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-01-16

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.22.6

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.22.5...n8n@1.22.6){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-01-10

This is a bug fix release. It includes important fixes for the HTTP Request and monday.com nodes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.24.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.23.0...n8n@1.24.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-01-10


This release contains new nodes for advanced AI, node enhancements, new features, performance enhancements, and bug fixes.

<div class="n8n-new-features" markdown>

#### Chat trigger

n8n has created a new [Chat Trigger node](/integrations/builtin/core-nodes/n8n-nodes-langchain.chattrigger/). The new node provides a chat interface that you can make publicly available, with customization and authentication options.

</div>

<div class="n8n-new-features" markdown>

#### Mistral Cloud Chat and Embeddings

This release introduces two new nodes to support [Mistral AI](https://mistral.ai/){:target=_blank .external-link}:

* [Mistral Cloud Chat Model](/integrations/builtin/cluster-nodes/sub-nodes/n8n-nodes-langchain.lmchatmistralcloud/)
* [Embeddings Mistral Cloud](/integrations/builtin/cluster-nodes/sub-nodes/n8n-nodes-langchain.embeddingsmistralcloud/)

</div>

### Contributors

[Anush](https://github.com/Anush008){:target=_blank .external-link}  
[Eric Koleda](https://github.com/ekoleda-codaio){:target=_blank .external-link}  
[Mason Geloso](https://github.com/MasonGeloso){:target=_blank .external-link}  
[vacitbaydarman](https://github.com/vacitbaydarman){:target=_blank .external-link}

## n8n@1.22.5

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.22.4...n8n@1.22.5){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-01-09

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.



## n8n@1.23.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.22.4...n8n@1.23.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-01-03

This release contains new nodes, node enhancements, new features, and bug fixes.

<div class="n8n-new-features" markdown>

#### New nodes and improved experience for working with files

This release includes a major overhaul of nodes relating to files (binary data).

There are now three key nodes dedicated to handling binary data files:

- [Read/Write Files from Disk](/integrations/builtin/core-nodes/n8n-nodes-base.filesreadwrite/) to read and write files from/to the machine where n8n is running.
- [Convert to File](/integrations/builtin/core-nodes/n8n-nodes-base.converttofile/) to take input data and output it as a file.
- [Extract From File](/integrations/builtin/core-nodes/n8n-nodes-base.extractfromfile/) to get data from a binary format and convert it to JSON.

n8n has moved support for iCalendar, PDF, and spreadsheet formats into these nodes, and removed the iCalendar, Read PDF, and Spreadsheet File nodes. There are still standalone nodes for [HTML](/integrations/builtin/core-nodes/n8n-nodes-base.html/) and [XML](/integrations/builtin/core-nodes/n8n-nodes-base.xml/).

</div>

<div class="n8n-new-features" markdown>

#### New node: Qdrant vector store

This release adds support for [Qdrant](https://qdrant.tech/){:target=_blank .external-link} with the Qdrant vector store node.

Read n8n's [Qdrant vector store node documentation](/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.vectorstoreqdrant/)

</div>

### Contributors



[Aaron Gutierrez](https://github.com/aarongut){:target=_blank .external-link}  
[Advaith Gundu](https://github.com/geodic){:target=_blank .external-link}  
[Anush](https://github.com/Anush008){:target=_blank .external-link}  
[Bin](https://github.com/soulhat){:target=_blank .external-link}  
[Nihaal Sangha](https://github.com/nihaals){:target=_blank .external-link}  



## n8n@1.22.4

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.22.3...n8n@1.22.4){:target=_blank .external-link} for this version.<br />
**Release date:** 2024-01-03



This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.22.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.22.2...n8n@1.22.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-12-27

/// note | Upgrade directly to 1.22.4
Due to issues with this release, upgrade directly to 1.22.4.
///

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.22.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.22.1...n8n@1.22.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-12-27

/// note | Upgrade directly to 1.22.4
Due to issues with this release, upgrade directly to 1.22.4.
///

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.22.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.22.0...n8n@1.22.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-12-21

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.22.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.21.1...n8n@1.22.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-12-21

This release contains node enhancements, new features, performance improvements, and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.18.4

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.18.3...n8n@1.18.4){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-12-19

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.21.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.20.0...n8n@1.21.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-12-15



This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.


## n8n@1.18.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.18.2...n8n@1.18.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-12-15

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.21.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.20.0...n8n@1.21.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-12-13

This release contains new features and nodes, node enhancements, and bug fixes.

<div class="n8n-new-features" markdown>

#### New user role: Admin

This release introduces a third account type: admin. This role is available on pro and enterprise plans. Admins have similar permissions to instance owners.

[Read more about user roles](/user-management/account-types/)

</div>

<div class="n8n-new-features" markdown>

#### New data transformation nodes

This release replaces the Item Lists node with a collection of nodes for data transformation tasks:

* [Aggregate](/integrations/builtin/core-nodes/n8n-nodes-base.aggregate/): take separate items, or portions of them, and group them together into individual items.
* [Limit](/integrations/builtin/core-nodes/n8n-nodes-base.aggregate/): remove items beyond a defined maximum number.
* [Remove Duplicates](/integrations/builtin/core-nodes/n8n-nodes-base.removeduplicates/): identify and delete items that are identical across all fields or a subset of fields.
* [Sort](/integrations/builtin/core-nodes/n8n-nodes-base.sort/): organize lists of in a desired ordering, or generate a random selection.
* [Split Out](/integrations/builtin/core-nodes/n8n-nodes-base.splitout/): separate a single data item containing a list into multiple items.
* [Summarize](/integrations/builtin/core-nodes/n8n-nodes-base.summarize/): aggregate items together, in a manner similar to Excel pivot tables. 

</div>

<div class="n8n-new-features" markdown>

#### Increased sharing permissions for owners and admins

Instance owners and users with the admin role can now see and share all workflows and credentials. They can't view sensitive credential information.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.20.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.19.5...n8n@1.20.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-12-06

This release contains bug fixes, node enhancements, and ongoing new feature work.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors


[Andrey Starostin](https://github.com/mayorandrew){:target=_blank .external-link}



## n8n@1.19.5

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.19.4...n8n@1.19.5){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-12-05

This is a bug fix release.

/// warning | Breaking change
This release removes the TensorFlow Embeddings node.
///

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.18.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.18.1...n8n@1.18.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-12-05

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.19.4

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.19.0...n8n@1.19.4){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-12-01

/// warning | Missing ARM v7 support
This version doesn't support ARM v7. n8n is working on fixing this in future releases.
///

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.19.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.18.0...n8n@1.19.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-11-29

/// note | Upgrade directly to 1.19.4
Due to issues with this release, upgrade directly to 1.19.4.
///

This release contains new features, node enhancements, and bug fixes.

<div class="n8n-new-features" markdown>

#### LangChain general availability

This release adds LangChain support to the main n8n version. Refer to [LangChain](/langchain/) for more information on how to build AI tools in n8n, the new nodes n8n has introduced, and related learning resources.

</div>

<div class="n8n-new-features" markdown>

#### Show avatars of users working on the same workflow

This release improves the experience of users collaborating on workflows. You can now see who else is editing at the same time as you.

</div>

## n8n@1.18.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.18.0...n8n@1.18.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-11-30

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.18.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.17.1...n8n@1.18.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-11-22

This release contains new features and bug fixes.

<div class="n8n-new-features" markdown>

#### Template creator hub

Built a template you want to share? This release introduces the n8n Creator hub. Refer to the [creator hub Notion doc](https://www.notion.so/n8n-Creator-hub-7bd2cbe0fce0449198ecb23ff4a2f76f){:target=_blank .external-link} for more information on this project.

</div>

<div class="n8n-new-features" markdown>

#### Node input and output search filter

Cloud Pro and Enterprise users can now search and filter the input and output data in nodes. Refer to [Data filtering](/data/data-filtering/) for more information.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.17.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.17.0...n8n@1.17.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-11-17

This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.17.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.16.0...n8n@1.17.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-11-15



This release contains node enhancements and bug fixes.

<div class="n8n-new-features" markdown>

#### Sticky Note Colors

You can now select background colors for sticky notes.

</div>

<div class="n8n-new-features" markdown>

#### Discord Node Overhaul

An overhaul of the Discord node, improving the UI making it easier to configure, improving error handling, and fixing issues.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors


[antondollmaier](https://github.com/antondollmaier){:target=_blank .external-link}  
[teomane](https://github.com/teomane){:target=_blank .external-link}  

## n8n@1.16.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.15.2...n8n@1.16.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-11-08

This release contains node enhancements and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.15.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.15.1...n8n@1.15.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-11-07

This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.15.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.14.2...n8n@1.15.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-11-02


This release contains new features, node enhancements, and bug fixes.

<div class="n8n-new-features" markdown>

#### Workflow history

This release introduces workflow history: view and load previous versions of your workflows. 

Workflow history is available in Enterprise n8n, and with limited history for Cloud Pro.

Learn more in the [Workflow history](/workflows/history/) documentation.

</div>

<div class="n8n-new-features" markdown>

#### Dark mode

_Almost_ in time for Halloween: this release introduces dark mode.

To enable dark mode:

1. Select **Settings** > **Personal**.
1. Under **Personalisation**, change **Theme** to **Dark theme**.

</div>

<div class="n8n-new-features" markdown>

#### Optional error output for nodes

All nodes apart from sub-nodes and trigger nodes have a new optional output: **Error**. Use this to add steps to handle node errors.

</div>

<div class="n8n-new-features" markdown>

#### Pagination support added to HTTP Request node

The HTTP Request node now supports an pagination. Read the [node docs](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) for information and examples.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Yoshino-s](https://github.com/Yoshino-s){:target=_blank .external-link}

## n8n@1.14.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.14.1...n8n@1.14.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-26

This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.14.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.14.0...n8n@1.14.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-26

This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.14.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.13.0...n8n@1.14.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-25

This release contains node enhancements and bug fixes.

<div class="n8n-new-features" markdown>

#### Switch node supports more outputs

The [Switch node](/integrations/builtin/core-nodes/n8n-nodes-base.switch/) now supports an unlimited number of outputs.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.13.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.12.2...n8n@1.13.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-25

This release contains new features, feature enhancements, and bug fixes.

/// note | Upgrade directly to 1.14.0
This release failed to publish to npm. Upgrade directly to 1.14.0.
///
<div class="n8n-new-features" markdown>

#### RSS Feed trigger node

This releases introduces a new node, the [RSS Feed Trigger](/integrations/builtin/core-nodes/n8n-nodes-base.rssfeedreadtrigger/). Use this node to start a workflow when a new RSS feed item is published.

</div>

<div class="n8n-new-features" markdown>

#### Facebook Lead Ads trigger node

This releases add another new node, the [Facebook Lead Ads Trigger](/integrations/builtin/trigger-nodes/n8n-nodes-base.facebookleadadstrigger/). Use this node to trigger a workflow when you get a new lead.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.12.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.12.1...n8n@1.12.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-24


This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Burak Akgün](https://github.com/mbakgun){:target=_blank .external-link}  

## n8n@1.12.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.12.0...n8n@1.12.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-23


This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Léo Martinez](https://github.com/martinezleoml){:target=_blank .external-link}  

## n8n@1.11.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.11.1...n8n@1.11.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-23

This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Inga](https://github.com/inga-lovinde){:target=_blank .external-link}  
[pemontto](https://github.com/pemontto){:target=_blank .external-link}  

## n8n@1.12.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.11.1...n8n@1.12.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-18

This release contains new features, node enhancements, and bug fixes.

<div class="n8n-new-features" markdown>

#### Form trigger node

This releases introduces a new node, the [n8n Form Trigger](/integrations/builtin/core-nodes/n8n-nodes-base.formtrigger/). Use this node to start a workflow based on a user submitting a form. It provides a configurable form interface.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Damian Karzon](https://github.com/dkarzon){:target=_blank .external-link}  
[Inga](https://github.com/inga-lovinde){:target=_blank .external-link}  
[pemontto](https://github.com/pemontto){:target=_blank .external-link}  


## n8n@1.11.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.11.0...n8n@1.11.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-13

This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.11.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.10.1...n8n@1.11.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-11


This release contains new features and bug fixes.

<div class="n8n-new-features" markdown>

#### External storage for binary files

Self-hosted users can now use an external service to store binary data. Learn more in [External storage](/hosting/external-storage/).

If you're using n8n Cloud and are interested in this feature, please [contact n8n](https://n8n-community.typeform.com/to/y9X2YuGa){:target=_blank .external-link}.

</div>

<div class="n8n-new-features" markdown>

#### Item Lists node supports binary data

The Item Lists node now supports splitting and concatenating binary data inputs. This means you no longer need to use code to split a collection of files into multiple items.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.10.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.10.0...n8n@1.10.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-11

This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.9.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.9.2...n8n@1.9.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-10

This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.9.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.9.1...n8n@1.9.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-09

This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.10.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.9.1...n8n@1.10.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-05



This release contains bug fixes and preparatory work for new features.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.


## n8n@1.9.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.9.0...n8n@1.9.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-10-04

This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## LangChain in n8n (beta)  

**Release date:** 2023-10-04

This release introduces support for building with LangChain in n8n. 

With n8n's LangChain nodes you can build AI-powered functionality within your workflows. The LangChain nodes are configurable, meaning you can choose your preferred agent, LLM, memory, and other components. Alongside the LangChain nodes, you can connect any n8n node as normal: this means you can integrate your LangChain logic with other data sources and services.

Read more:

* This is a beta release, and not yet available in the main product. Follow the instructions in [Access LangChain in n8n](/langchain/access-langchain/) to try it out. Self-hosted and Cloud options are available.
* Learn how LangChain concepts map to n8n nodes in [LangChain concepts in n8n](/langchain/langchain-n8n/).
* Browse n8n's new [Cluster nodes](/integrations/builtin/cluster-nodes/). This is a new set of node types that allows for multiple nodes to work together to configure each other.
* If you want to take a look at the code, it's available on the [ai-beta](https://github.com/n8n-io/n8n/tree/ai-beta){:target=_blank .external-link} in the n8n repository. Note that it may move in the future.


## n8n@1.9.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.8.2...n8n@1.9.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-09-28


This release contains new features, performance improvements, and bug fixes.

--8<-- "_snippets/code/tournament-notes.md"

<div class="n8n-new-features" markdown>

#### Tournament

This releases replaces RiotTmpl, the templating language used in expressions, with n8n's own templating language, [Tournament](https://github.com/n8n-io/tournament){:target=_blank .external-linmk}. You can now use arrow functions in expressions.<br />

</div>

<div class="n8n-new-features" markdown>

#### `N8N_BINARY_DATA_TTL` and `EXECUTIONS_DATA_PRUNE_TIMEOUT` removed

The environment variables `N8N_BINARY_DATA_TTL` and `EXECUTIONS_DATA_PRUNE_TIMEOUT` no longer have any effect and can be removed. Instead of relying on a TTL system for binary data, n8n cleans up binary data together with executions during pruning.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.8.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.8.1...n8n@1.8.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-09-25




This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.8.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.8.0...n8n@1.8.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-09-21


This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.8.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.7.1...n8n@1.8.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-09-20

This release contains node enhancements and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.7.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.7.0...n8n@1.7.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-09-14


This release contains bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.7.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.6.1...n8n@1.7.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-09-13

This release contains node enhancements and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Quang-Linh LE](https://github.com/linktohack){:target=_blank .external-link}  
[MC Naveen](https://github.com/mcnaveen){:target=_blank .external-link}

## n8n@1.6.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.6.0...n8n@1.6.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-09-06


This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.6.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.5.1...n8n@1.6.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-09-06

This release contains bug fixes, new features, and node enhancements.

/// note | Upgrade directly to 1.6.1
Skip this version and upgrade directly to 1.6.1, which contains essential bug fixes.
///
<div class="n8n-new-features" markdown>

#### TheHive 5

This release introduces support for TheHive API version 5. This uses a new node and credentials:

* [TheHive 5 node](/integrations/builtin/app-nodes/n8n-nodes-base.thehive5/)
* [TheHive 5 trigger node](/integrations/builtin/trigger-nodes/n8n-nodes-base.thehive5trigger/)
* [TheHive 5 credentials](/integrations/builtin/credentials/thehive5/)

#### `N8N_PERSISTED_BINARY_DATA_TTL` removed

The environment variables `N8N_PERSISTED_BINARY_DATA_TTL` no longer has any effect and can be removed. This legacy flag was originally introduced to support ephemeral executions (see [details](https://github.com/n8n-io/n8n/pull/7046)), which are no longer supported.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.5.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.5.0...n8n@1.5.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-08-31


This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.5.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.4.1...n8n@1.5.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-08-31

This release contains new features, node enhancements, and bug fixes.

/// note | Upgrade directly to 1.5.1
Skip this version and upgrade directly to 1.5.1, which contains essential bug fixes.
///
### Highlights

<div class="n8n-new-features" markdown>

#### External secrets storage for credentials

Enterprise-tier accounts can now use external secrets vaults to manage credentials in n8n. This allows you to store credential information securely outside your n8n instance. n8n supports Infisical and HashiCorp Vault.

Refer to [External secrets](/external-secrets/) for guidance on enabling and using this feature.

</div>

<div class="n8n-new-features" markdown>

#### Two-factor authentication

n8n now supports two-factor authentication (2FA) for self-hosted instances. n8n is working on bringing support to Cloud. Refer to [Two-factor authentication](/user-management/two-factor-auth/) for guidance on enabling and using it.

</div>

<div class="n8n-new-features" markdown>

#### Debug executions

Users on a paid n8n plan can now load data from previous executions into their current workflow. This is useful when debugging a failed execution.

Refer to [Debug executions](/workflows/executions/debug/) for guidance on using this feature.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.4.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.4.0...n8n@1.4.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-08-29



This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.4.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.3.1...n8n@1.4.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-08-23

This release contains new features, node enhancements, and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[pemontto](https://github.com/pemontto){:target=_blank .external-link}

## n8n@1.3.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.3.0...n8n@1.3.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-08-18

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.237.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.236.3...n8n@0.237.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-08-17

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Jordan Hall](https://github.com/Jordan-Hall){:target=_blank .external-link}  
[Xavier Calland](https://github.com/xavier-calland){:target=_blank .external-link}

## n8n@1.3.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.2.2...n8n@1.3.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-08-16

This release contains new features and bug fixes.

### Highlights

<div class="n8n-new-features" markdown>

#### Trial feature: AI support in the Code node

This release introduces limited support for using AI to generate code in the Code node. Initially this feature is only available on Cloud, and will gradually be rolled out, starting with about 20% of users.

Learn how to use the feature, including guidance on writing prompts, in [Generate code with ChatGPT](/code/ai-code/).

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Ian Gallagher](https://github.com/craSH){:target=_blank .external-link}  
[Xavier Calland](https://github.com/xavier-calland){:target=_blank .external-link}

## n8n@1.2.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.2.1...n8n@1.2.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-08-14

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.2.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.2.0...n8n@1.2.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-08-09


This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.2.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.1.1...n8n@1.2.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-08-09

This release contains new features, node enhancements, bug fixes, and performance improvements.

/// note | Upgrade directly to 1.2.1
When upgrading, skip this release and go directly to 1.2.1.
///
### Highlights

<div class="n8n-new-features" markdown>

#### Credential support for SecOps services

This release introduces support for setting up credentials in n8n for the following services:

* [AlienVault](/integrations/builtin/credentials/alienvault/)
* [Auth0 Management](/integrations/builtin/credentials/auth0management/)
* [Carbon Black API](/integrations/builtin/credentials/carbonblack/)
* [Cisco Meraki API](/integrations/builtin/credentials/ciscomeraki/)
* [Cisco Secure Endpoint](/integrations/builtin/credentials/ciscosecureendpoint/)
* [Cisco Umbrella API](/integrations/builtin/credentials/ciscoumbrella/)
* [CrowdStrike](/integrations/builtin/credentials/crowdstrike/)
* [F5 Big-IP](/integrations/builtin/credentials/f5bigip/)
* [Fortinet FortiGate](/integrations/builtin/credentials/fortigate/)
* [Hybrid Analysis](/integrations/builtin/credentials/hybridanalysis/)
* [Imperva WAF](/integrations/builtin/credentials/impervawaf/)
* [Kibana](/integrations/builtin/credentials/kibana/)
* [Microsoft Entra ID](/integrations/builtin/credentials/microsoftentra/)
* [Mist](/integrations/builtin/credentials/mist/)
* [Okta](/integrations/builtin/credentials/okta/)
* [OpenCTI](/integrations/builtin/credentials/opencti/)
* [QRadar](/integrations/builtin/credentials/qradar/)
* [Qualys](/integrations/builtin/credentials/qualys/)
* [Recorded Future](/integrations/builtin/credentials/recordedfuture/)
* [Sekoia](/integrations/builtin/credentials/sekoia/)
* [Shuffler](/integrations/builtin/credentials/shuffler/)
* [Trellix ePO](/integrations/builtin/credentials/trellixepo/)
* [VirusTotal](/integrations/builtin/credentials/virustotal/)
* [Zscaler ZIA](/integrations/builtin/credentials/zscalerzia/)

This makes it easier to do [Custom operations](/integrations/custom-operations/) with these services, using the [HTTP Request](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) node.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.1.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.1.0...n8n@1.1.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-07-27


This is a bug fix release.

/// warning | Breaking changes
Please note that this version contains breaking changes if upgrading from a `0.x.x` version. For full details, refer to the [n8n v1.0 migration guide](/1-0-migration-checklist/).
///
For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.1.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.0.5...n8n@1.1.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-07-26

This release contains new features, bug fixes, and node enhancements.

/// warning | Breaking changes
Please note that this version contains breaking changes if upgrading from a `0.x.x` version. For full details, refer to the [n8n v1.0 migration guide](/1-0-migration-checklist/).
///
### Highlights

<div class="n8n-new-features" markdown>

#### Source control and environments

This release introduces source control and environments for enterprise users.

n8n uses Git-based source control to support environments. Linking your n8n instances to a Git repository lets you create multiple n8n environments, backed by Git branches.

Refer to [Source control and environments](/source-control-environments/) to learn more about the features and set up your environments.

</div>

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Adrián Martínez](https://github.com/adrian-martinez-vdshop){:target=_blank .external-link}  
[Alberto Pasqualetto](https://github.com/albertopasqualetto){:target=_blank .external-link}  
[Marten Steketee](https://github.com/Marten-S){:target=_blank .external-link}  
[perseus-algol](https://github.com/perseus-algol){:target=_blank .external-link}  
[Sandra Ashipala](https://github.com/sandramsc){:target=_blank .external-link}  
[ZergRael](https://github.com/ZergRael){:target=_blank .external-link}  

## n8n@1.0.5

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.0.4...n8n@1.0.5){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-07-24



This is a bug fix release.

/// warning | Breaking changes
Please note that this version contains breaking changes if upgrading from a `0.x.x` version. For full details, refer to the [n8n v1.0 migration guide](/1-0-migration-checklist/).
///
For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.0.4

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.0.3...n8n@1.0.4){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-07-19


This is a bug fix release.

/// warning | Breaking changes
Please note that this version contains breaking changes if upgrading from a `0.x.x` version. For full details, refer to the [n8n v1.0 migration guide](/1-0-migration-checklist/).
///
For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Romain Dunand](https://github.com/airmoi){:target=_blank .external-link}  
[noctarius aka Christoph Engelbert](https://github.com/noctarius){:target=_blank .external-link}

## n8n@0.236.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.236.2...n8n@0.236.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-07-18

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Romain Dunand](https://github.com/airmoi){:target=_blank .external-link}  
[noctarius aka Christoph Engelbert](https://github.com/noctarius){:target=_blank .external-link}

## n8n@0.236.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.236.1...n8n@0.236.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-07-14

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.0.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.0.2...n8n@1.0.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-07-13

This release contains API enhancements and adds support for sending messages to forum threads in the Telegram node.

/// warning | Breaking changes
Please note that this version contains breaking changes if upgrading from a `0.x.x` version. For full details, refer to the [n8n v1.0 migration guide](/1-0-migration-checklist/).
///
For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Kirill](https://github.com/chrtkv){:target=_blank .external-link}

## n8n@0.236.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.236.0...n8n@0.236.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-07-12

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@1.0.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.0.1...n8n@1.0.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-07-05

This is a bug fix release.

/// warning | Breaking changes
Please note that this version contains breaking changes if upgrading from a `0.x.x` version. For full details, refer to the [n8n v1.0 migration guide](/1-0-migration-checklist/).
///
### Contributors

[Romain Dunand](https://github.com/airmoi){:target=_blank .external-link}

## n8n@1.0.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@1.0.0...n8n@1.0.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-07-05

/// warning | Breaking changes
Please note that this version contains breaking changes. For full details, refer to the [n8n v1.0 migration guide](/1-0-migration-checklist/).
///
This is n8n's version one release.

For full details, refer to the [n8n v1.0 migration guide](/1-0-migration-checklist/).

### Highlights

<div class="n8n-new-features" markdown>

#### Python support

Although JavaScript remains the default language, you can now also select Python as an option in the [Code node](/code/code-node/) and even make use of [many Python modules](https://pyodide.org/en/stable/usage/packages-in-pyodide.html#packages-in-pyodide){:target=_blank .external link}. Note that Python is unavailable in Code nodes added to a workflow before v1.0.

</div>

### Contributors

[Marten Steketee](https://github.com/Marten-S){:target=_blank .external-link}


## n8n@0.236.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.235.0...n8n@0.236.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-07-05


This release contains new nodes, node enhancements, and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### New nodes

<div class="n8n-new-features" markdown>

#### crowd.dev

This release includes a [crowd.dev](https://www.crowd.dev/){:target=_blank .external-link} node and crowd.dev trigger node. crowd.dev is a tool to help you understand who is engaging with your open source project.

[crowd.dev node documentation](/integrations/builtin/app-nodes/n8n-nodes-base.crowddev/).

</div>

### Contributors

[Alberto Pasqualetto](https://github.com/albertopasqualetto){:target=_blank .external-link}  
[perseus-algol](https://github.com/perseus-algol){:target=_blank .external-link}  
[Romeo Balta](https://github.com/romeobalta){:target=_blank .external-link}  
[ZergRael](https://github.com/ZergRael){:target=_blank .external-link}  

## n8n@0.234.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.234.0...n8n@0.234.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-07-05

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.235.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.234.0...n8n@0.235.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-06-28

This release contains new features, new nodes, node enhancements, and bug fixes.

/// warning | Unstable version
This version is (as of 4th July 2023) considered unstable. n8n recommends against upgrading.
///
For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Contributors

[Marten Steketee](https://github.com/Marten-S){:target=_blank .external-link}  
[Sandra Ashipala](https://github.com/sandramsc){:target=_blank .external-link}

## n8n@0.234.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.233.1...n8n@0.234.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-06-22

This release contains new features, new nodes, node enhancements, and bug fixes.	

/// warning | Unstable version
This version is (as of 4th July 2023) considered unstable. n8n recommends upgrading directly to 0.234.1.	
///
/// warning | Irreversible database migration
This version contains a database migration that changes credential and workflow IDs to use nanoId strings, This migration may take a while to complete in some environments. This change doesn't break anything using the older numeric IDs.

If you upgrade to 0.234.0, you can't roll back to an earlier version.
///


For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### New nodes

<div class="n8n-new-features" markdown>

#### Debug Helper

The Debug Helper node can be used to trigger different error types or generate random datasets to help test n8n workflows.

[Debug Helper node documentation](/integrations/builtin/core-nodes/n8n-nodes-base.debughelper/).

</div>

## n8n@0.233.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.233.0...n8n@0.233.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-06-19

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.233.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.232.0...n8n@0.233.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-06-14


This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.232.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.231.1...n8n@0.232.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-06-07

This release contains new features, new nodes, node enhancements, and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### New nodes

This release includes a new trigger node for Postgres, which allows you to listen to events, as well as listen to custom channels. Refer to [Postgres trigger](/integrations/builtin/trigger-nodes/n8n-nodes-base.postgrestrigger/) for more information.

## n8n@0.231.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.231.2...n8n@0.231.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-06-17




This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.231.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.231.1...n8n@0.231.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-06-14

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.


## n8n@0.231.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.231.0...n8n@0.231.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-06-06


This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.231.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.230.2...n8n@0.231.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-05-31

This release contains bug fixes and new features.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### New features

Notable new features.

#### Resource mapper UI component

This release includes a new UI component, the resource mapper. This component is useful for node creators. If your node does insert, update, or upsert operations, you need to send data from the node in a format supported by the service you're integrating with. Often it's necessary to use a Set node before a node that sends data, to get the data to match the schema of the service you're connecting to. The resource mapper UI component provides a way to get data into the required format directly within the node.

Refer to [Node user interface elements | Resource mapper](/integrations/creating-nodes/build/reference/ui-elements/#resource-mapper) for guidance for node builders.

## n8n@0.230.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.230.2...n8n@0.230.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-06-05

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.230.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.230.1...n8n@0.230.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-05-25

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.230.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.230.0...n8n@0.230.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-05-25

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.230.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.229.0...n8n@0.230.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-05-24

This release contains new features, new nodes, node enhancements, and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### New nodes

<div class="n8n-new-features" markdown>

#### Execution Data

Save metadata for workflow executions. You can then search by this data in the **Executions** list.

[Execution Data node documentation](/integrations/builtin/core-nodes/n8n-nodes-base.executiondata/).

</div>

<div class="n8n-new-features" markdown>

#### LDAP node

The LDAP node allows you to interact with your LDAP servers from your n8n workflows. 

[LDAP node documentation](/integrations/builtin/core-nodes/n8n-nodes-base.ldap/).

</div>

<div class="n8n-new-features" markdown>

#### LoneScale node

Integrate n8n with [LoneScale](https://www.lonescale.com/){:target=_blank .external-link}, a buying intents data platform.

[LoneScale node documentation](/integrations/builtin/app-nodes/n8n-nodes-base.lonescale/).

</div>

### Contributors

[Bram Kn](https://github.com/bramkn){:target=_blank .external-link}  
[pemontto](https://github.com/pemontto){:target=_blank .external-link}  
[Yann Aleman](https://github.com/SanYann){:target=_blank .external-link}

## n8n@0.229.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.228.0...n8n@0.229.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-05-17

This release contains bug fixes, improves UI copy and error messages in some nodes, and other node enhancements.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Node enhancements

The Google Ads node now supports v13.


## n8n@0.228.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.228.1...n8n@0.228.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-05-15


This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.228.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.228.0...n8n@0.228.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-05-11

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.228.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.227.0...n8n@0.228.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-05-11

This release contains new features, node enhancements, and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### New nodes

<div class="n8n-new-features" markdown>

#### npm node

This release introduces the [npm](/integrations/builtin/app-nodes/n8n-nodes-base.npm/) node. This is a new core node. It provides a way to query an npm registry within your workflow.

</div>

### Contributors

[Adam Charnock](https://github.com/adamcharnock){:target=_blank .external-link}

## n8n@0.227.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.227.0...n8n@0.227.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-05-15

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.


## n8n@0.227.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.226.2...n8n@0.227.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-05-03

This release contains new features, node enhancements, and bug fixes.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### Node enhancements

* An overhaul of the Microsoft Excel 365 node, improve the UI making it easier to configure, improve error handling, and fix issues.

### Deprecations

This release deprecates the following:

* The `EXECUTIONS_PROCESS` environment variable.
* Running n8n in own mode. Main mode is now the default. Use [Queue mode](/hosting/scaling/queue-mode/) if you need full execution isolation.
* The `WEBHOOK_TUNNEL_URL` flag. Replaced by `WEBHOOK_URL`.
* Support for MySQL and MariaDB as n8n backend databases. n8n will remove support completely in version 1.0. n8n recommends using PostgreSQL instead.

## n8n@0.226.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.226.1...n8n@0.226.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-05-03

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.226.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.226.0...n8n@0.226.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-05-02

This is a bug fix release.

For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

## n8n@0.226.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.225.2...n8n@0.226.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-26

This release contains new features, node enhancements, and bug fixes.

/// warning | Breaking changes
Please note that this version contains a breaking change to `extractDomain` and `isDomain`. You can read more about it [here](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#02260){:target=_blank .external-link}.
///
For full release details, refer to [Releases](https://github.com/n8n-io/n8n/releases){:target=_blank .external-link} on GitHub.

### New features

* A new command to get information about licenses for self-hosted users: 
	```sh
	n8n license:info
	```

### Node enhancements

* Nodes that use SQL, such as the PostgresSQL node, now have a better SQL editor for writing custom queries.
* An overhaul of the Google BigQuery node to support executing queries, improve the UI making it easier to configure, improve error handling, and fix issues.

## n8n@0.225.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.225.1...n8n@0.225.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-25

This is a bug fix release.

### Bug fixes

* Core: Upgrade google-timezones-json to use the correct timezone for Sao Paulo.
* Code Node: Update vm2 to address [CVE-2023-30547](https://github.com/advisories/GHSA-ch3r-j5x3-6q2m){:target=_blank .external-link}.

## n8n@0.225.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.225.0...n8n@0.225.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-20

This is a bug fix release.

### Bug fixes

* Editor: Clean up demo and template callouts from workflows page.
* Editor: Fix memory leak in Node Detail View by correctly unsubscribing from event buses.
* Editor: Settings sidebar should disconnect from push when navigating away.
* Notion Node: Update credential test to not require user permissions.



## n8n@0.225.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.224.1...n8n@0.225.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-19

### New features

<div class="n8n-new-features" markdown>

This release introduces [Variables](/code/variables/). You can now create variables that allows you to store and reuse values in n8n workflows. This is the first phase of a larger project to support [Environments](/source-control-environments/) in n8n.

</div>

* Core: Add support for Google Service account authentication in the HTTP Request node.
* GitLab Node: Add **Additional Parameters** for the file list operation.
* MySQL Node: This node has been overhauled.

### Bug fixes

* Core: Fix broken API permissions in public API.
* Core: Fix paired item returning wrong data.
* Core: Improve SAML connection test result views.
* Core: Make getExecutionId available on all nodes types.
* Core: Skip SAML onboarding for users with first- and lastname.
* Editor: Add padding to prepend input.
* Editor: Clean up demo/video experiment.
* Editor: Enterprise features missing with user management.
* Editor: Fix moving canvas on middle click preventing lasso selection.
* Editor: Make sure to redirect to blank canvas after personalisation modal.
* Editor: Fix an issue that was preventing typing certain characters in the UI on devices with touchscreen.
* Editor: Fix n8n-checkbox alignment.
* Code Node: Handle user code returning null and undefined.
* GitHub Trigger Node: Remove content_reference event.
* Google Sheets Trigger Node: Return actual error message.
* HTTP Request Node: Fix `itemIndex` in HTTP Request errors.
* NocoDB Node: Fix for updating or deleting rows with not default primary keys.
* OpenAI Node: Update models to only show those supported.
* OpenAI Node: Update OpenAI Text Moderate input placeholder text.

### Contributors

[Bram Kn](https://github.com/bramkn){:target=_blank .external-link}  
[Eddy Hernandez](https://github.com/eddywashere){:target=_blank .external-link}  
[Filipe Dobreira](https://github.com/filp){:target=_blank .external-link}  
[Jimw383](https://github.com/Jimw383){:target=_blank .external-link}  

## n8n@0.224.4

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.224.2...n8n@0.224.4){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-24

This is a bug fix release.

### Bug fixes

* Core: Upgrade google-timezones-json to use the correct timezone for Sao Paulo.
* Code Node: Update vm2 to address [CVE-2023-30547](https://github.com/advisories/GHSA-ch3r-j5x3-6q2m){:target=_blank .external-link}.


## n8n@0.224.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.224.1...n8n@0.224.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-20

This is a bug fix release.

### Bug fixes

* Core: Fix paired item returning wrong data.
* Core: Make getExecutionId available on all nodes types.
* Editor: Fix memory leak in Node Detail View by correctly unsubscribing from event buses.
* Editor: Fix moving canvas on middle click preventing lasso selection.
* Editor: Settings sidebar should disconnect from push when navigating away.
* Google Sheets Trigger Node: Return actual error message.
* HTTP Request Node: Fix `itemIndex` in HTTP Request errors.
* Notion Node: Update credential test to not require user permissions.

### Contributors


[Filipe Dobreira](https://github.com/filp){:target=_blank .external-link}


## n8n@0.224.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.224.0...n8n@0.224.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-14

This is a bug fix release.

### Bug fixes

* Core: Fix broken API permissions in public API.
* Editor: Fix an issue that was preventing typing certain characters in the UI on devices with touchscreen.

## n8n@0.224.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.223.0...n8n@0.224.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-12

This release contains a new node, updates, and bug fixes.

### New nodes

This release introduces the [TOTP](/integrations/builtin/core-nodes/n8n-nodes-base.totp/) node. This is a new core node. It provides a way to generate a TOTP (time-based one-time password) within your workflow.

### Bug fixes

* Code Node: Update vm2 to address CVE-2023-29017.
* Core: App shouldn't crash with a custom REST endpoint.
* Core: Do not execute workflowExecuteBefore hook when resuming executions from a waiting state.
* Core: Fix issue where sub workflows would display as running forever after failure to start.
* Core: Update xml2js to address CVE-2023-0842.
* Editor: Drop mergeDeep in favor of lodash merge.
* HTTP Request Node: Restore detailed error message.

### Contributors


[Loganaden Velvindron](https://github.com/loganaden){:target=_blank .external-link}


## n8n@0.223.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.222.1...n8n@0.223.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-05

This release contains new features and bug fixes.

/// warning | Breaking changes
Please note that this version contains a breaking change. The minimum Node.js version is now v16. You can read more about it [here](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#02230){:target=_blank .external-link}.
///

### New features

* Core: Convert `eventBus` controller to decorator style and improve permissions.
* Core: Prevent non owners password reset when SAML is enabled (this is preparation for an upcoming feature).
* Core: Read ephemeral license from environment and clean up `ee` flags.
* Editor: Allow tab to accept completion.
* Editor: Enable saving workflow when node details view is open.
* Editor: SSO onboarding (this is preparation for an upcoming feature).
* Editor: SSO setup (this is preparation for an upcoming feature).

### Node enhancements

* Filter Node: Show discarded items.
* HTTP Request Node: Follow redirects by default.
* Postgres Node: Overhaul node.
* ServiceNow Node: Add support for work notes when updating an incident.
* SSH Node: Hide the private key within the SSH credential.

### Bug fixes

* Add droppable state for booleans when mapping.
* Compare Datasets Node: Fuzzy comparen't comparing keys missing in one of the inputs.
* Compare Datasets Node: Fix support for dot notation in skip fields.
* Core: Deactivate active workflows during import.
* Core: Stop marking duplicates as circular references in `jsonStringify`.
* Core: Stop using `util.types.isProxy` for tracking of augmented objects.
* Core: Fix curl import error when no data.
* Core: Handle Date and RegExp correctly in `jsonStringify`.
* Core: Handle Date and RegExp objects in `augmentObject`.
* Core: Prevent `augmentObject` from creating infinitely deep proxies.
* Core: Service account private key as a password field.
* Core: Update lock file.
* Core: Waiting workflows not stopping.
* Date & Time Node: Add info box at top of date and time explaining expressions.
* Date & Time Node: Convert Luxon DateTime object to ISO.
* Editor: Add `$if`, `$min`, `$max` to root expression autocomplete.
* Editor: Curb overeager item access linting.
* Editor: Disable Grammarly in expression editors.
* Editor: Disable password reset on desktop with no user management.
* Editor: Fix connection lost hover text not showing.
* Editor: Fix issue preventing execution preview loading when in an Iframe.
* Editor: Fix mapping with special characters.
* Editor: Prevent error from showing-up when duplicating unsaved workflow.
* Editor: Prevent NDV schema view pagination.
* Editor: Support backspacing with modifier key.
* Google Sheets Node: Fix insertOrUpdate cell update with object.
* HTML Extract Node: Support for dot notation in JSON property.
* HTTP Request Node: Fix AWS credentials to stop removing URL parameters for STS.
* HTTP Request Node: Refresh token properly on never fail option.
* HTTP Request Node: Support for dot notation in JSON body.
* LinkedIn Node: Update the version of the API.
* Redis Node: Fix issue with hash set not working as expected.



## n8n@0.222.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.222.2...n8n@0.222.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-14

This is a bug fix release.

### Bug fixes

* Core: Fix broken API permissions in public API.
* Editor: Fix an issue that was preventing typing certain characters in the UI on devices with touchscreen.

## n8n@0.222.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.222.1...n8n@0.222.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-11

This is a bug fix release.

### Bug fixes

* Code node: Update vm2 to address CVE-2023-29017.
* Core: Update xml2js to address CVE-2023-0842.

### Contributors


[Loganaden Velvindron](https://github.com/loganaden){:target=_blank .external-link}

## n8n@0.222.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.222.0...n8n@0.222.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-04

This is a bug fix release.

### Bug fixes

* AWS SNS Node: Fix an issue with messages failing to send if they contain certain characters.
* Core: `augmentObject` should clone Buffer/Uint8Array instead of wrapping them in a proxy.
* Core: `augmentObject` should use existing property descriptors whenever possible.
* Core: Fix the issue of nodes not loading when run using npx.
* Core: Improve Axios error handling in nodes.
* Core: Password reset should pass in the correct values to external hooks.
* Core: Prevent `augmentObject` from creating infinitely deep proxies.
* Core: Use table-prefixes in queries in import commands.
* Editor: Fix focused state in Code node editor.
* Editor: Fix loading executions in long execution list.
* Editor: Show correct status on canceled executions.
* Gmail Node: Gmail Luxon object support, fix for timestamp.
* HTTP Request Node: Detect mime-type from streaming responses.
* HubSpot Trigger Node: Developer API key is required for webhooks.
* Set Node: Convert string to number.

## n8n@0.222.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.221.2...n8n@0.222.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-03-30

This release contains new features, including custom filters for the executions list, and a new node to filter items in your workflows.

/// note | Upgrade to 0.222.1
Upgrade directly to 0.222.1.
///
### New features

<div class="n8n-new-features" markdown>

This release introduces improvements to the execution lists. You can now save [Custom execution data](/workflows/executions/custom-executions-data/), and use it to filter both the [All executions](/workflows/executions/all-executions/) and [Single workflow executions](/workflows/executions/single-workflow-executions/) lists.

</div>


* Add test overrides.
* Core: Improve LDAP/SAML toggle and tests.
* Core: Limit user invites when SAML is enabled.
* Core: Make OAuth2 error handling consistent with success handling.
* Editor: Fix ResourceLocator dropdown style.


### New nodes

This release introduces the [Filter](/integrations/builtin/core-nodes/n8n-nodes-base.filter/) node. The node allows you to filter items based on a condition. If the item meets the condition, the Filter node passes it on to the next node in the Filter node output. If the item doesn't meet the condition, the Filter node omits the item from its output.

### Bug fixes

* Core: Assign `properties.success` earlier to set `executionStatus` correctly.
* Core: Don't mark duplicates as circular references in `jsonStringify`.
* Core: Don't use `util.types.isProxy` for tracking of augmented objects.
* Core: Ensure that all non-lazy-loaded community nodes get post-processed correctly.
* Core: Force-upgrade decode-uri-component to address CVE-2022-38900.
* Core: Force-upgrade http-cache-semantics to address CVE-2022-25881.
* Core: Handle `Date` and `RegExp` correctly in `jsonStringify`.
* Core: Handle `Date` and `RegExp` objects in `augmentObject`.
* Core: Improve Axios error handling in nodes.
* Core: Improve community nodes loading.
* Core: Initialize queue in the webhook server as well.
* Core: Persist `CurrentAuthenticationMethod` setting change.
* Core: Remove circular references from Code and push message.
* Core: Require authentication on icons and nodes/credentials types static files.
* Core: Return SAML service provider URls with configuration.
* Core: Service account private key should display as a password field.
* Core: Upgrade Luxon to address CVE-2023-22467.
* Core: Upgrade simple-git to address CVE-2022-25912.
* Core: Upgrade SQLite3 to address CVE-2022-43441.
* Core: Upgrade Convict to address CVE-2023-0163.
* Core: Waiting workflows not stopping.
* Editor: Fix connection lost hover text not showing.
* Editor: Fix issue preventing execution preview loading when in an iframe.
* Editor: Use credentials when fetching node and credential types.
* Google Sheets Node: Fix `insertOrUpdate` cell update with object.
* HTTP Request Node: Add streaming to binary response.
* HTTP Request Node: Fix AWS credentials to automatically deconstruct the URL.
* HTTP Request Node: Fix AWS credentials to stop removing URL parameters for STS.
* Split In Batches Node: Roll back changes in v1 and create v2.
* Update PostHog no-capture.


### Contributors


[Manish Dhanwal](https://github.com/ManishDhanwal07){:target=_blank .external-link}


## n8n@0.221.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.221.2...n8n@0.221.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-04-11

This is a bug fix release.

### Bug fixes

* Code node: Update vm2 to address CVE-2023-29017.
* Core: Update xml2js to address CVE-2023-0842.

### Contributors


[Loganaden Velvindron](https://github.com/loganaden){:target=_blank .external-link}

## n8n@0.221.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.221.1...n8n@0.221.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-03-24

This is a bug fix release. It fixes an issue with `properties.success` that was causing `executionStatus` to sometimes be incorrect.



## n8n@0.221.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.221.0...n8n@0.221.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-03-23

This is a bug fix release. It ensures the job queue is initiated before starting the webhook server.


## n8n@0.221.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.220.1...n8n@0.221.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-03-23

### New features

* Core: n8n now augments data rather than copying it in the Code node. This is a performance improvement.
* Editor: you can now move the canvas by holding `Space` and dragging with the mouse, or by holding the middle mouse button and dragging.
* Editor: add authentication type recommendations in the credentials modal.
* Editor: add the SSO login button.

### New nodes

This release adds a node for [QuickChart](https://quickchart.io/){:target=_blank .external-link}, an open source chart generation tool.

### Bug fixes

* Core: ensure n8n calls available error workflows in main mode recovery.
* Core: fix telemetry execution status for manual workflows executions.
* Core: return SAML attributes after connection test.
* Editor: disable mapping tooltip for display modes that don't support mapping.
* Editor: fix execution list item selection.
* Editor: fix for large notifications being cut off.
* Editor: fix redo in code and expression editor.
* Editor: fix the canvas node distance when automatically injecting manual trigger.
* HTTP Request Node: fix AWS credentials to automatically deconstruct the URL.
* Split In Batches Node: roll back changes in v1 and create v2.




## n8n@0.220.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.220.0...n8n@0.220.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-03-22

This is a bug fix release. It reverts changes to version 1 of the Split In Batches node, and creates a version 2 containing the updates.



## n8n@0.220.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.219.1...n8n@0.220.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-03-16

This release adds schema view to the node output panel, and includes node enhancements and bug fixes.

### New features

* Core: improve SAML connection test.
* Editor: add basic Datatable and Pagination components.
* Editor: add support for schema view in the NDV output.
* Editor: don't show actions panel for single-action nodes.

### Node enhancements

* Item Lists Node: update actions text.
* OpenAI Node: add support for GPT4 on chat completion.
* Split In Batches Node: make it easier to combine processed data.

### Bug fixes

* Core: initialize license and LDAP in the correct order.
* Editor: display correct error message for `$env` access.
* Editor: fix autocomplete for complex expressions.
* Editor: fix owner set-up checkbox wording.
* Editor: properly handle mapping of dragged expression if it contains hyphen.
* Metabase Node: fix issue with question results not correctly being returned.



## n8n@0.219.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.219.0...n8n@0.219.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-03-10

This is a bug fix release. It resolves an issue with the HTTP Request node by removing the streaming response.


## n8n@0.219.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.218.0...n8n@0.219.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-03-09

### New features

* Core: add `advancedFilters` feature flag.
* Core: add SAML post and test endpoints.
* Core: add SAML XML validation.
* Core: limit user changes when SAML is enabled.
* Core: refactor and add SAML preferences for service provider instance.
* Editor: don't automatically add the manual trigger when the user adds another node.
* Editor: redirect users to canvas if they don't have any workflows.

### Node enhancements

* Cal Trigger Node: update to support v2 webhooks.
* HTTP Request Node: move from binary buffer to binary streaming.
* Mattermost Node: add self signed certificate support.
* Microsoft SQL Node: add support for self signed certificates.
* Mindee Node: add support for v4 API.
* Slack Node: move from binary buffer to binary streaming.

### Bug fixes

* Core: allow serving icons for custom nodes with npm scoped names.
* Core: rename `advancedFilters` to `advancedExecutionFilters`.
* Editor: fix ElButton overrides.
* Editor: only fetch new versions at app launch.
* Fetch credentials on workflows view to include in duplicated workflows.
* Fix color discrepancies for executions list items.
* OpenAI Node: fix issue with expressions not working with chat complete.
* OpenAI Node: simplify code.

### Contributors


[Syed Ali Shahbaz](https://github.com/alishaz-polymath){:target=_blank .external-link}



## n8n@0.218.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.217.2...n8n@0.218.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-03-02

This release contains node enhancements, bug fixes, and new features that lay groundwork for upcoming releases, along with some UX improvements.

### New features

* Add distribution test tracking.
* Add events to enable onboarding checklist.
* Core: add SAML login setup (for upcoming feature).
* Core: add SAML settings and consolidate LDAP under SSO (for upcoming feature).
* Editor: add missing documentation to autocomplete items for inline code editor.
* Editor: Show parameter hint on multiline inputs.

### Node enhancements

* JIRA node: support binary streaming for very large binary files.
* OpenAI node: add support for ChatGPT.
* Telegram node: add parse mode option to Send Document operation.

### Bug fixes

* Core: fix execution pruning queries.
* Core: fix filtering workflow by tags.
* Core: revert isPending check on the user entity.
* Fix issues with nodes missing in nodes panel.
* Fix mapping paths when appending to empty expression.
* Item Lists Node: tweak item list summarize field naming.
* Prevent executions from displaying as running forever.
* Show Execute Workflow node in the nodes panel.
* Show RabbitMQ node in the nodes panel.
* Stop showing mapping hint after mapping.




## n8n@0.217.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.217.1...n8n@0.217.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-27

This is a bug fix release.

### Bug fixes

* Core: fix issue with execution pruning queries.
* Core: fix for workflow filtering by tag.
* Core: revert isPending check on the user entity.





## n8n@0.217.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.217.0...n8n@0.217.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-24

This is a bug fix release.

### Bug fixes

Prevent executions appearing to run forever.





## n8n@0.217.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.216.1...n8n@0.217.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-23

This release contains new features and bug fixes. It includes improvements to the nodes panel and executions list. It also deprecates the Read Binary File node.


### New features

* Add new event hooks to support telemetry around the new onboarding experience.
* Update nodes to set required path type.
* Core: add configurable execution history limit. Use this to improve performance when self-hosting. Refer to [Execution Data | Enable data pruning ](/hosting/scaling/execution-data#enable-data-pruning) for more information.
* Core: add execution runData recovery and status field. This allows us to show execution statuses on the **Executions** list.
* Core: add SAML feature flag. This is preparatory for an upcoming feature.
* Editor: improvements to the nodes panel search. When searching in root view, n8n now displays results from both trigger and regular nodes. When searching in a category view, n8n shows results from the category, and also suggests results from other categories.
* Hide sensitive value in authentication header credentials and authentication query credentials.
* Support feature flag evaluation server side.
* Deprecate the Read Binary File node. Use the [Read Binary Files](/integrations/builtin/core-nodes/n8n-nodes-base.readbinaryfiles/) node instead.


### Bug fixes

* Baserow Node: fix issue with **Get All** not correctly using filters.
* Compare Datasets Node: UI tweaks and fixes.
* Core: don't allow arbitrary path traversal in BinaryDataManager.
* Core: don't allow arbitrary path traversal in the credential-translation endpoint.
* Core: don't explicitly bypass authentication on URLs containing `.svg`.
* Core: don't remove empty output connections arrays in PurgeInvalidWorkflowConnections migration.
* Core: fix execution status filters.
* Core: user update endpoint should only allow updating email, firstName, and lastName.
* Discord Node: fix wrong error message being displayed.
* Discourse Node: fix issue with credential test not working.
* Editor: apply correct IRunExecutionData to finished workflow.
* Editor: fix an issue with zoom and canvas nodes connections.
* Editor: fix unexpected date rendering on front-end.
* Editor: remove `crashed` status from filter.
* Fix typo in error messages when a property doesn't exist.
* Fixes an issue when saving an active workflow without triggers would cause n8n to be stuck.
* Google Calendar Node: fix incorrect labels for start and end times when getting all events.
* Postgres Node: fix for tables containing field named JSON.
* AWS S3 Node: fix issue with get many buckets not outputting data.

--8<-- "_snippets/update-n8n.md"


## n8n@0.216.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.216.2...n8n@0.216.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-03-09

This is a bug fix release. It reverts the `isPending` check on the user entity, resolving an issue with displaying user options when user management is disabled.



## n8n@0.216.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.216.1...n8n@0.216.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-23

This is a bug fix release.

### Bug fixes

Core: don't remove empty output connections arrays in PurgeInvalidWorkflowConnections migration.


## n8n@0.215.4

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.215.3...n8n@0.215.4){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-03-14

This is a bug fix release. It reverts the `isPending` check on the user entity, resolving an issue with displaying user options when user management is disabled.

--8<-- "_snippets/update-n8n.md"


## n8n@0.215.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.215.2...n8n@0.215.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-23

This is a bug fix release. It contains an important security fix.

### Bug fixes

* Core: don't allow arbitrary path traversal in BinaryDataManager.
* Core: don't allow arbitrary path traversal in the credential-translation endpoint.
* Core: don't explicitly bypass authentication on URLs containing `.svg`.
* Core: don't remove empty output connections arrays in PurgeInvalidWorkflowConnections migration.
* Core: the user update endpoint should only allow updating email, first name, and last name.


## n8n@0.214.5

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.214.4...n8n@0.214.5){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-03-14

This is a bug fix release. It reverts the `isPending` check on the user entity, resolving an issue with displaying user options when user management is disabled.

--8<-- "_snippets/update-n8n.md"


## n8n@0.214.4

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.214.3...n8n@0.214.4){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-23

This is a bug fix release. It contains an important security fix.

### Bug fixes

* Core: don't allow arbitrary path traversal in BinaryDataManager.
* Core: don't allow arbitrary path traversal in the credential-translation endpoint.
* Core: don't explicitly bypass authentication on URLs containing `.svg`.
* Core: don't remove empty output connections arrays in PurgeInvalidWorkflowConnections migration.
* Core: the user update endpoint should only allow updating email, first name, and last name.






## n8n@0.216.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.216.0...n8n@0.216.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-21

This is a bug fix release.

### Bug fixes

* Core: don't allow arbitrary path traversal in BinaryDataManager.
* Core: don't allow arbitrary path traversal in the credential-translation endpoint.
* Core: don't explicitly bypass auth on URLs containing `.svg`.
* Core: user update endpoint should only allow updating email, firstName, and lastName.





## n8n@0.216.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.215.2...n8n@0.216.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-16

This release contains new features, node enhancements, and bug fixes.

### New features

* Add workflow and credential sharing access e2e tests.
* Editor: add correct credential owner contact details for readonly credentials.
* Editor: add most important native properties and methods to autocomplete.
* Editor: update to personalization survey v4.
* Update telemetry API endpoints.

### Node enhancements

* GitHub node: update code to use resource locator component.
* GitHub trigger node: update code to use resource locator component.
* Notion node: add option to set icons when creating pages or database pages.
* Slack node: add support for manually inputting a channel name for channel operations.

### Bug fixes

* Core: fix data transformation functions.
* Core: remove unnecessary info from GET `/workflows` response.
* Bubble node: fix pagination issue when returning all objects.
* HTTP Request Node: ignore empty body when auto-detecting JSON.

### Contributors


[feelgood-interface](https://github.com/feelgood-interface){:target=_blank .external-link}




## n8n@0.215.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.215.1...n8n@0.215.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-14

This is a bug fix release. It solves an issue that was causing webhooks to be removed when they shouldn't be.



## n8n@0.215.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.215.0...n8n@0.215.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-11

This is a bug fix release.

### Bug fixes

* Core: fix issue causing worker and webhook service to close on start.
* Core: handle versioned custom nodes correctly.





## n8n@0.215.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.214.3...n8n@0.215.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-10

This release contains new features, node enhancements, and bug fixes.

### New features

* Refactor the n8n Desktop user management experience.
* Core: add support for WebSockets as an alternative to server-sent events. This introduces a new way for n8n's backend to push changes to the UI. The default is still server-sent events. If you're experiencing issues with the UI not updating, try changing to WebSockets by setting the `N8N_PUSH_BACKEND` environment variable to `websocket`. 
* Editor: add autocomplete for objects.
* Editor: add autocomplete for expressions to the HTML editor component.


### Node enhancements

* Edit Image node: add support for WebP image format.
* HubSpot trigger node: add conversation events.


### Bug fixes

* Core: disable transactions on SQLite migrations that use PRAGMA foreign_keys.
* Core: ensure expression extension doesn't fail with optional chaining.
* Core: fix import command for workflows with old format (affects workflows created before user management was introduced).
* Core: stop copying icons to cache.
* Editor: prevent creation of input connections for nodes without input slot.
* Error workflow now correctly checks for subworkflow permissions.
* ActiveCampaign Node: fix additional fields not being sent when updating account contacts.
* Linear Node: fix issue with Issue States not loading correctly.
* MySQL migration parses database contents if necessary (fix for MariaDB).

### Contributors


[Kirill](https://github.com/chrtkv){:target=_blank .external-link}



## n8n@0.214.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.214.2...n8n@0.214.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-09

This is a bug fix release.

### Bug fixes

Editor: prevent creation of input connections for nodes without input slot.





## n8n@0.214.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.214.1...n8n@0.214.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-06

This is a bug fix release.

### Bug fixes

* Editor: correctly show OAuth reconnect button.
* Editor: fix resolvable highlighting for HTML editor.





## n8n@0.214.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.214.0...n8n@0.214.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-06

This is a bug fix release. It also contains an overhaul of the Slack node.

### Node enhancements

This release includes an overhaul of the Slack node, adding new operations and a better user interface.

### Bug fixes

* Editor: fix an issue with mapping to empty expression input.
* Editor: fix merge node connectors.
* Editor: fix multiple-output endpoints success style after connection is detached.





## n8n@0.214.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.213.0...n8n@0.214.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-02-03

This release contains new features, node enhancements, and bug fixes. The expressions editor now supports autocomplete for some [built in data transformation functions](/code/builtin/data-transformation-functions/). The new features also include two of interest to node builders: a way to allow users to drag and drop data keys, and the new HTML editor component.

/// warning | Breaking changes
Please note that this version contains a breaking change to Luxon. You can read more about it [here](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#02140){:target=_blank .external-link}.
///
### New features

<div class="n8n-new-features" markdown>

#### Autocomplete in the Extension editor

[Data transformation functions](/code/builtin/data-transformation-functions/) now have autocomplete support in the Expression editor.

</div>

* Core: export OpenAPI spec for external tools.
* Core: set custom Cache-Control headers for static assets.
* Core: simplify pagination in declarative node design.
* Editor: support mapping keys with drag and drop. Any field with the hint **Enter the field name as text** should now support mapping a data key using drag and drop. Node builders can enable this in their own nodes. Refer to [Creating nodes | UI elements](/integrations/creating-nodes/build/reference/ui-elements#support-drag-and-drop-for-data-keys) for more information.
* Editor: add the [HTML editor component](/integrations/creating-nodes/build/reference/ui-elements#html) for use in parameters. This means node builders can now use the HTML editor that n8n uses in the HTML node as a UI component.
* Editor: append expressions in fixed values when mapping to string and JSON inputs.
* Editor: continue to show mapping tooltip after dismiss.
* Editor: roll out schema view.


### Node enhancements

* FTP Node: stream binary data for uploads and downloads.
* Notion Node: add support for image blocks.
* OpenAI Node: add **Frequency Penalty** and **Presence Penalty** to the node options for the text resource.
* Salesforce Node: add **Has Opted Out Of Email** field to lead resource options.
* SSH Node: stream binary data for uploads and downloads.
* Write Binary File Node: stream binary data for writes.
* YouTube Node: switch upload operation over to streaming and resumable uploads API.

### Bug fixes

* Add paired item to the most used nodes.
* Core: fix OAuth2 client credentials not always working.
* Core: fix populating of node custom API call options.
* Core: fix value resolution in declarative node design.
* Core: prevent shared user details being saved alongside execution data.
* Core: revert custom API option injecting.
* Editor: add SMTP info translation link slot.
* Editor: change executions title to match menu.
* Editor: fix JSON field completions while typing.
* Editor: handling router errors when navigation is canceled by user.
* Editor: set max width for executions list.
* Editor: stop unsaved changes popup display when navigating away from an untouched workflow.
* Editor: fix workflow executions view.
* Invoice Ninja Node: fix line items not being correctly set for quotes and invoices.
* Linear Node: fix pagination issue for get all issues.
* Mailchimp Trigger Node: fix webhook recreation.
* Prevent unnecessarily touching `updatedAt` when n8n starts.
* Schedule Trigger Node: change scheduler behaviour for intervals days and hours.
* Set Node: fix behaviour when selecting `continueOnFail` and `pairedItem`.





## n8n@0.213.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.212.1...n8n@0.213.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-01-27

This release introduces LDAP, and a new node for working with HTML in n8n. It also contains node enhancements and bug fixes.

### New features

<div class="n8n-new-features" markdown>

#### LDAP

This release introduces support for LDAP on Self-hosted Enterprise and Cloud Enterprise plans. Refer to [LDAP](/user-management/ldap/) for more information on this feature.

</div>

* Simplify the Node Details View by moving authentication details to the Credentials modal.
* Improve workflow list performance.

### New nodes

<div class="n8n-new-features" markdown>

#### HTML node

n8n has a new [HTML node](/integrations/builtin/core-nodes/n8n-nodes-base.html/). This replaces the HTML Extract node, and adds new functionality to generate HTML templates.

</div>

### Node enhancements

* GitLab node: add file resource and operations.
* JIRA Software node: introduce the resource locator component to improve UX.
* Send Email node: this node has been overhauled.

### Bug fixes

* Core: don't crash express app on unhandled rejected promises.
* Core: handle missing binary metadata in download URLs.
* Core: upsert (update and insert) credentials and workflows in the `import:` commands.
* Core: validate numeric IDs in the public API.
* Editor: don't request workflow data twice when opening a workflow.
* Editor: execution list micro optimization.
* Editor: fix node authentication options ordering and hiding options based on node version.
* Editor: fix save modal appearing after duplicating a workflow.
* Editor: prevent workflow execution list infinite no network error.
* Extension being too eager and making calls when it shouldn't.
* Google Drive Node: use the correct MIME type on converted downloads.
* HelpScout Node: fix tag search not working when getting all conversations.
* Notion (Beta) Node: fix create database page with multiple relation IDs not working.
* Update **Sign in with Google** button to properly match design guidelines.

### Contributors


* [Devin Buhl](https://github.com/onedr0p){:target=_blank .external-link} 
* [Sven Ziegler](https://github.com/svzi){:target=_blank .external-link} 


## n8n@0.212.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.212.0...n8n@0.212.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-01-23

This release includes an overhaul of the Google Analytics node, and bug fixes.

### Node enhancements

This release includes an overhaul of the Google Analytics node. This brings the node's code and components in line with n8n's latest node building styles, and adds support for GA4 properties.

### Bug fixes

* Add schema to Postgres migrations.
* Core: fix execute-once incoming data handling.
* Core: fix expression extension miss-detection.
* Core: fix onWorkflowPostExecute not being called.
* Core: fix URL in error handling for the error Trigger.
* Core: make pinned data with webhook responding on last node manual-only.
* Editor: making parameter input components label configurable.
* Editor: remove infinite loading in not found workflow level execution.
* Linear Node: fix issue with single item not being returned.
* Notion (Beta) Node: fix create database page fails if relation parameter is empty/undefined.





## n8n@0.212.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.211.2...n8n@0.212.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-01-19

This release contains enhancements to the Item Lists node, and bug fixes.

### New features

This release adds experimental support for more Prometheus metrics. Self-hosting users can configure Prometheus using [environment variables](/hosting/environment-variables/environment-variables/).

### Node enhancements

<div class="n8n-new-features" markdown>

The [Item Lists node](/integrations/builtin/core-nodes/n8n-nodes-base.itemlists/) now supports a Summarize operation. This acts similarly to generating pivot tables in Excel, allowing you to aggregate and compare data.

</div>

### Bug fixes

* Core: revert a lint rule `@typescript-eslint/prefer-nullish-coalescing`.
* Editor: allow special characters in node selector completion.
* GitLab Node: update the credential test endpoint.
* Gmail Trigger Node: resolve an issue that was preventing filter by labels from working.
* HTTP Request Node: ensure node enforces the requirement for valid JSON input.
* HTTP Request Node: convert responses to text for all formats, including JSON.

### Contributors


[Sven Ziegler](https://github.com/svzi){:target=_blank .external-link}


## n8n@0.211.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.211.1...n8n@0.211.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-01-17

This release contains a bug fix for community nodes, and a new trigger node.

### New nodes

<div class="n8n-new-features" markdown>

#### Google Sheets trigger node

This release adds a new [Google Sheets trigger node](/integrations/builtin/trigger-nodes/n8n-nodes-base.googlesheetstrigger/). You can now start workflows in response to row changes or new rows in a Google Sheet.

</div>

### Bug fixes

Fixes an issue that was preventing users from installing community nodes.


## n8n@0.211.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.211.0...n8n@0.211.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-01-16

This is a bug fix release. It resolves major issues with 0.211.0.

### New features

Editor: suppress validation errors for freshly added nodes.

### Node enhancements

* Google Ads node: update the API version to 11.
* Google Drive Trigger node: start using the resource locator component.

### Bug fixes

* Build CLI to fix Postgres and MySQL test runs.
* Extend date functions clobbering plus/minus.
* Extension deep comparen't quite working for some primitives.
* Upgrade jsonwebtoken to address CVE-2022-23540.





## n8n@0.211.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.210.2...n8n@0.211.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-01-13

/// warning | Don't use this version
Upgrade directly to 0.211.1.
///
### New features

* Add demo experiment to help users activate.
* Editor: Improvements to the **Executions** page.
* Editor: Remove prevent-ndv-auto-open feature flag.
* Editor: Update callout component design.
* Add the expression extension framework.

### Bug fixes

* Core: Fixes event message confirmations if no subscribers present.
* Core: Remove threads package, rewrite log writer worker.
* Core: Throw error in UI on expression referencing missing node but don't fail execution.
* DB revert command shouldn't run full migrations before each revert.
* Editor: Disable data pinning on multiple output node types.
* Editor: Don't overwrite `window.onerror` in production.
* Editor: Execution page bug fixes.
* Editor: Fixes event bus test.
* Editor: Hide data pinning discoverability tooltip in execution view.
* Editor: Mapping tooltip dismiss.
* Editor: Recover from unsaved finished execution.
* Editor: Setting NDV session ID.
* First/last being extended on proxy objects.
* Handle memory issues gracefully.
* PayPal Trigger Node: Omit verification in sandbox environment.
* Report app startup and database migration errors to Sentry.
* Run every database migration inside a transaction.
* Upgrade class-validator to address CVE-2019-18413.
* Zoom Node: Add notice about deprecation of Zoom JWT app support.

### Known issues

You may encounter errors when using the [optional chaining operator](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Optional_chaining){:target=_blank .external-link} in expressions. If this happens, avoid using the operator for now.





## n8n@0.210.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.210.1...n8n@0.210.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-01-09

### New features

<div class="n8n-new-features" markdown>

#### Typeahead for expressions

When using [expressions](/code/expressions/), n8n will now offer you suggestions as you type.

!["Animated GIF showing typeahead in action"](/_images/reference/release-notes/0.210.2-expressions-type-ahead.gif)

</div>

### Bug fixes

* Core: fix crash of manual workflow executions for unsaved workflows.
* Editor: omit pairedItem from proxy completions.
* Editor: prevent refresh on submit in credential edit modal.
* Google Sheets Node: fix for auto-range detection.
* Read Binary File Node: don't crash the execution when the source file doesn't exist.
* Remove anonymous ID from tracking calls.
* Stop OOM crashes in Execution Data pruning.
* Update links for user management and SMTP help.



## n8n@0.210.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.210.0...n8n@0.210.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-01-05

This is a bug fix release. It also contains a new feature to support user management without SMTP set up.

### New features

#### Invite link for users on self-hosted n8n

In earlier versions of self-hosted n8n, you needed SMTP set up on your n8n instance for user management to work. User management required SMTP to sent invitation emails.

0.210.1 introduces an invite link, which you can copy and send to users manually. n8n still recommends setting up SMTP, as this is needed for password resets.

### Bug fixes

* Google Sheets node: fix an issue that was causing append and update operations to fail for numeric values.
* Resolve issues with external hooks.

## n8n@0.210.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.209.4...n8n@0.210.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2023-01-05

This release introduces two major new features: log streaming and security audits. It also contains node enhancements, bug fixes, and performance improvements.

### New features

<div class="n8n-new-features" markdown>

#### Log streaming

This release introduces [log streaming](/log-streaming/) for users on Enterprise self-hosted plans and custom Cloud plans. Log streaming allows you to send events from n8n to your own logging tools. This allows you to manage your n8n monitoring in your own alerting and logging processes.

</div>

<div class="n8n-new-features" markdown>

#### Security audit

This release adds a [security audit](/hosting/security-audit/) feature. You can now run a security audit on your n8n instance, to detect common security issues.

</div>

* Core: add support for Redis 6+ ACLs system using username in queue mode. Add the `QUEUE_BULL_REDIS_USERNAME` environment variable.

### Node enhancements

* Compare Datasets node: add an option for fuzzy compare.

### Bug fixes

* Apply credential overwrites recursively. This ensures that overwrites defined for a parent credential type also apply to all credentials extending it.
* Core: enable full manual execution of a workflow using the error trigger.
* Core: fix OAuth credential creation using the API.
* Core: fix an issue with workflow lastUpdated field.
* Editor: clear node creator and scrim on workspace reset.
* Editor: fix an infinite loop while loading executions that aren't on the current executions list.
* Editor: make node title non-editable in executions view.
* Editor: prevent scrim on executable triggers.
* Editor: support tabbing away from inline expression editor.
* Fix executions bulk deletion.
* Google Sheets Node: fix exception when no **Values to Send** are set.
* Respond to Webhook Node: fix issue that caused the content-type header to be overwritten.
* Slack Node: add missing channels:read OAuth2 scope.

### Performance improvements

* Lazy-load public API dependencies to reduce baseline memory usage.
* Lazy-load queue mode and analytics dependencies.

### Contributors


[Thomas S.](https://github.com/intel44){:target=_blank .external-link}

## n8n@0.209.4

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.209.3...n8n@0.209.4){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-12-28

This is primarily a bug fix release.

### Bug fixes

* Editor: add sticky note without manual trigger.
* Editor: display default missing value in table view as undefined.
* Editor: fix displaying of some trigger nodes in the creator panel.
* Editor: fix trigger node type identification on add to canvas.
* Editor: add the usage and plans page to Desktop.

### New features

Editor: pressing **=** in an empty parameter input switches to expression mode.

## n8n@0.209.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.209.2...n8n@0.209.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-12-27

This is primarily a bug fix release.

### Bug fixes

* Core: don't send credentials to browser console.
* Core: permit a workflow user who isn't the owner to use their own credentials.
* Editor: fix for loading executions that aren't on the current executions list.
* Editor: make the tertiary button on the **Usage** page transparent.
* Editor: update credential owner warning when sharing.

### New features

Editor: Improve UX for brace completion in the inline expressions editor.

### Node enhancements

Webhook node: when test the node by selecting **Listen For Test Event** then dispatching a call to the webhook, n8n now only runs the Webhook node. Previously, n8n ran the entire workflow. You can still test the full workflow by selecting **Test Workflow**, then dispatching a test call. 

## n8n@0.209.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.209.1...n8n@0.209.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-12-23

This is a bug fix release.

### Bug fixes

* Editor: ensure full tree on expression editor parse. This resolves an issue with the expressions editor cutting off results.
* Fix automatic credential selection when credentials are shared.

### Performance improvements

Improvements to the workflows list performance.

## n8n@0.209.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.209.0...n8n@0.209.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-12-22

This is a bug fix release.

### Bug fixes

* Editor: fix for executions preview scroll load bug and wrong execution being displayed.
* Editor: force parse on long expressions.
* Editor: restore trigger to the nodes panel.
* Nodes: AWS DynamoDB Node Fix issue pagination and simplify issue.
* Nodes: fix DynamoDB node type issues.
* Resolve an issue with credentials and workflows not being matched correctly due to incorrect typing.
* Restore missing tags when retrieving a workflow.

### Contributors


[Nathan Apter](https://github.com/napter){:target=_blank .external-link}

## n8n@0.209.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.208.1...n8n@0.209.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-12-21

This release introduces workflow sharing, and changes to licensing and payment plans.

### New features

<div class="n8n-new-features" markdown>

#### Workflow sharing

This release introduces workflow sharing for users on some plans. With workflow sharing, users can invite other users on the same n8n instance to use and edit their workflows. Refer to [Workflow sharing](/workflows/sharing/) for details.

</div>

### Bug fixes

* Editor: Correctly display trigger nodes without actions and with related regular node in the "On App Events" category.
* Fix stickies resize.
* Hide trigger tooltip for nodes with static test output.
* Keep expression when dropping mapped value.
* Prevent keyboard shortcuts in expression editor modal.
* Redirect home to workflows always.
* Update mapping GIFs.
* Upgrade amqplib to address CVE-2022-0686.
* View option for binary-data shouldn't download the file on Chrome/Edge.



## n8n@0.208.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.208.0...n8n@0.208.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-12-19

This is a bug fix release.

### Bug fixes

* Always retain original errors in the error chain on NodeOperationError.
* BinaryDataManager should store metadata when saving from buffer.
* Editor: fix for wrong execution data displayed in executions preview.
* Pick up credential test functions from versioned nodes.

## n8n@0.208.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.207.1...n8n@0.208.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-12-16

This release introduces a new inline expressions editor, and a new node: OpenAI. It also contains updates and bug fixes.

### New features

<div class="n8n-new-features" markdown>

#### Inline expression editor

You can now quickly write expressions inline in a node parameter. You can still choose to open the full expressions editor.

!["Screenshot of the inline expressions editors"](/_images/reference/release-notes/0.208.0-inline-expressions.png)

</div>

* Add workflow sharing telemetry.
* Core: allow for hiding page usage with environment variables (for upcoming feature)
* Editor: update UI copy for user management setup when sharing is disabled.
* Editor: hide credentials password values.
* Editor: set **All workflows** view as default view on the **Workflows** page.
* Editor: update UI copy for workflow overwriting message.

### New nodes

<div class="n8n-new-features" markdown>

#### Open AI node

This release adds an integration with OpenAI. Refer to the [OpenAI node documentation](/integrations/builtin/app-nodes/n8n-nodes-base.openai/) for details.

</div>

### Node enhancements

Send Email node: add support for a "Reply to" email address.

### Bug fixes

* Core: fix for Google and Microsoft generic OAuth2 credentials.
* Core: fix HTTP Digest Auth for responses without an opaque parameter.
* Disqus node: fix thread parameter for "Get All Threads" operation.
* Don't crash the server when Telemetry is blocked using DNS.
* Editor: allow mapping onto expression editor with selection range.
* Editor: don't show actions dialog for actionless triggers when selected using keyboard.
* Editor: fix an issue where some node actions wouldn't select default parameters correctly.
* Editor: fix typo in retry-button option "Retry with original workflow".
* Update permission for showing workflow caller policy.
* Update pnpm-lock to fix build.

### Contributors


[Daemonxiao](https://github.com/Daemonxiao){:target=_blank .external-link}  
[Kirill](https://github.com/kirill-chertkov){:target=_blank .external-link}  
[Ricardo Duarte](https://github.com/rduarte){:target=_blank .external-link}  


## n8n@0.207.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.207.0...n8n@0.207.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-12-13

This is a bug fix release. It resolves an issue with undo.

## n8n@0.207.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.206.1...n8n@0.207.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-12-12

This release adds support for undo/redo actions on the canvas, and includes bug fixes.

### New features

<div class="n8n-new-features" markdown>

#### Undo/redo

You can now undo and redo actions on the canvas.

Use `ctrl`/`cmd` + `z` to undo, `ctrl`/`cmd` + `shift` + `z` to redo.

Currently, n8n supports undo/redo for the following canvas actions:

- Adding nodes
- Deleting nodes
- Adding connections
- Deleting connections
- Moving nodes
- Moving connections
- Import workflow (from file/from URL)
- Copy/paste nodes
- Renaming nodes
- Duplicating nodes
- Disabling/enabling nodes

</div>

* App integration actions are now displayed in the nodes pane.
* Add sharing permissions info for workflow sharees.
* Handle sharing features when the user skips instance owner setup.
* Update the credential test error message for credential sharees.

### Bug fixes

* Core: remove nodeGetter.
* Core: Increase workflow reactivation max timeout to one day.
* Core: Resolve an issue listing executions with Postgres.
* Core: Remove foreign credentials when copying nodes or duplicating workflow.
* Core: upgrade sse-channel to mitigate CVE-2019-10744.
* Core: use license-sdk v1.6.1.
* Editor: avoid adding manual trigger node when webhook node is added.
* Editor: fix credential sharing issues handler when no matching ID or name.
* Editor: fix for broken tab navigation.
* Editor: schema view shows checkbox in case of empty data.
* Editor: Stop returning UNKNOWN ERROR in the response if an actual error message is available.
* Editor: update duplicate workflow action.
* Move Binary Data Node: stringify objects before encoding them in MoveBinaryData.
* Split In Batches Node: fix issue with pairedItem.


## n8n@0.206.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.206.0...n8n@0.206.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-12-06

This is a bug fix release.

### Bug fixes

* Core: make expression resolution improvements.
* Editor: schema unit test stub for Font Awesome icons.
* Remove unnecessary console message.

## n8n@0.206.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.205.0...n8n@0.206.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-12-06

This release contains bug fixes, node enhancements, and a new node input view: schema view.

### New features

<div class="n8n-new-features" markdown>

#### Schema view

Schema view is a new node input view. It helps you browse the structure of your data, using the first input item.

</div>

* Core: add workflow execution statistics.
* Editor: add the alert design system component.
* Editor: fix checkbox line hight and make checkbox label clickable.
* Nodes: add a message for read-only nodes.
* Nodes: add a prompt to overwrite changes when concurrent editing occurs.

### Node enhancements

KoBo Toolbox node: add support for the media file API.

### Bug fixes

* Core: fix linter error.
* Core: fix partial execution with pinned data on child node run.
* Core: OAuth2 scopes now save.
* Enable source-maps on WorkflowRunnerProcess in own mode.
* Handle error when workflow doesn'texist or is inaccessible.
* Make nodes.exclude and nodes.include work with lazy-loaded nodes.
* Code Node: restore `pairedItem` to required n8n item keys.
* Execute Workflow Node: update Execute Workflow node info notice text.
* Gmail Trigger Node: trigger node missing some emails.
* Local File Trigger Node: fix issue that causes a crash if the ignore field is empty.


### Contributors


[Marcel](https://github.com/marzn){:target=_blank .external-link}  
[Yann Jouanique](https://github.com/Yann-J){:target=_blank .external-link}  

## n8n@0.205.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.204.0...n8n@0.205.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-12-02

This release contains an overhaul of the expressions editor, node enhancements, and bug fixes.

### New features

<div class="n8n-new-features" markdown>

#### Expressions editor usability overhaul

This release contains usability enhancements for the expressions editor. The editor now includes color signals to indicate when syntax is valid or invalid, and better error messages and tips.

</div>

### Node enhancements

* Facebook Graph APInode: update to support API version 15.
* Google Calendar node: introduce the resource locator component to help users retrieve calendar parameters.
* Postmark trigger node: update credentials so they can be used with the HTTP Request node (for custom API calls).
* Todoist node: update to use API version 2.

### Bug fixes

* Core: ensure executions list is properly filtered for all users.
* Core: fix `$items().length` in Execute Once mode.
* Core: mark binary data to be deleted when pruning executions.
* Core: OAuth2 scope saved to database fix.
* Editor: fix slots rendering of NodeCreator's NoResults component.
* Editor: JSON view values can be mapped like keys.
* AWS SNS Node: fix a pagination issue.
* Google Sheets Node: fix exception if no matching rows are found.
* Google Sheets Node: fix for append operation if no empty rows in sheet.
* Microsoft Outlook Node: fix binary attachment upload.
* Pipedrive Node: resolve properties not working.
* Lazy load nodes for credentials testing.
* Credential overwrites should take precedence over credential default values.
* Remove background for resource ownership selector.
* Update padding for resource filters dropdown.
* Update size of select components in filters dropdown.
* Update workflow save button type and design and share button type.


## n8n@0.204.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.203.1...n8n@0.204.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-11-24

This release contains performance enhancements and bug fixes.

### New features

* Core: lazy-load nodes and credentials to reduce baseline memory usage.
* Core: use longer stack traces when error reporting is enabled.
* Dev: add credentials E2E test suite and page object.

### Bug fixes

* Core: fix $items().length behavior in executeOnce mode.
* Core: fix for unused imports.
* Core: use CredentialsOverwrites when testing credentials.
* Core: disable workflow locking due to issues.
* Editor: fix for missing node connections in dev environment.
* Editor: fix missing resource locator component.
* Editor: prevent node-creator tabs from showing when toggled by CanvasAddButton.
* Editor: table view column limit tooltip.
* Editor: fix broken n8n-info-tip slots.
* IF Node: fix "Is Empty" and "Is Not Empty" operation failures for date objects.
* Remove redundant `await` in nodes API request functions without try/catch.
* Schedule Trigger Node: fixes inconsistent behavior with cron and weekly intervals.
* Workflow activation shouldn't crash if one of the credential is invalid.

## n8n@0.203.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.203.0...n8n@0.203.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-11-18

This is a bug fix release. It resolves an issue with the Google Sheets node versioning.

## n8n@0.203.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.202.1...n8n@0.203.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-11-17

This release includes an overhaul of the Google Sheets node, as well as other new features, node enhancements, and bug fixes.

### New features

* Add duplicate workflow error handler.
* Add workflow data reset action.
* Add credential runtime checks and prevent tampering during a manual run.

### Node enhancements

* Compare Datasets: UI copy changes to improve usability.
* Google Sheets: n8n has overhauled this node, including improved lookup for document and sheet selection.
* Notion (beta) node: use the resource locator component for database and page parameters.

### Bug fixes

* Core: deduplicate error handling in nodes.
* Editor: show back mapping hint when parameter is focused.
* Editor: add **Stop execution** button to execution preview.
* Editor: curb direct item access linting.
* Editor: fix expression editor variable selector filter.
* Editor: fix for execution retry dropdown not closing.
* Editor: fix for logging error on user logout.
* Editor: fix zero treated as missing value in resource locator.
* Editor: hide pin data in production executions.
* Editor: skip optional chaining operators in Code Node editor linting.
* Editor: update to **Expression/Fixed** toggle - keep expression when switching to **Fixed**.
* Editor: fix foreign credentials being shown for new nodes.
* Editor: store copy of workflow in `workflowsById` to prevent node data bugs.
* Editor: fix user redirect to signin bug.

## n8n@0.202.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.202.0...n8n@0.202.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-11-10

This is a bug fix release. It removes some error tracking.

## n8n@0.202.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.201.0...n8n@0.202.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-11-10

This release contains core product improvements and bug fixes.

### New features

* API: report unhandled app crashes using Sentry.
* API: set up error tracking using Sentry.
* Core: Add ownership, sharing and credential details to `GET /workflows` in n8n's internal API.
* Editor: when building nodes, you can now add a property with type `notice` to your credentials `properties`.This was previously available in nodes but not credentials. Refer to [Node UI elements](/integrations/creating-nodes/build/reference/ui-elements/) for more information.

### Bug fixes

* API: Don't use names for type ORM connections.
* Core: Fix manual execution of pinned trigger on main mode.
* Core: Streamline multiple pinned triggers behavior.
* Editor: Curb argument linting for `$input.first()` and `$input.last()`
* Editor: Fix duplicate bug when new workflow is open.
* Editor: Fix for incorrect execution saving indicator in executions view.
* Editor: Fix for OAuth authorization.
* Editor: Fix workflow activation from the Workflows view.
* Editor: Fix workflow back button navigation.
* Editor: Prevent adding of the start node when importing workflow in the demo mode.
* Editor: Show string numbers and null properly in JSON view.
* Editor: Switch CodeNodeEditor linter parser to esprima-next.
* Editor: Tweak dragged mapping state.
* Editor: Update workflow buttons spacings.
* Editor: Use base path in workflow preview component URL.
* HTTP Request Node: Show error cause in the output.
* HTTP Request Node: Use the data in **Put Output in Field** field.
* HubSpot Node: Add notice to HubSpot credentials about API Key Sunset.
* Notion Trigger (Beta) Node: Fix Notion trigger polling strategy.
* Raindrop Node: Update access token URL.
* SendInBlue Trigger Node: Fix typo in credential name.
* Update E2E testing ENV variables.

### Contributors


[feelgood-interface](https://github.com/feelgood-interface){:target=_blank .external-link}  
[Ugo Bataillard](https://github.com/knshiro){:target=_blank .external-link}


## n8n@0.201.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.200.1...n8n@0.201.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-11-02

This release contains workflow and node enhancements, and bug fixes.

### New features

* Core: reimplement blocking workflow updates on interim changes.
* Editor: block the UI in node details view when the workflow is listening for an event.
* Performance improvements

### Node enhancements

Venafi TLS Protect Cloud node: make issuing template depend on application.

### Bug fixes

* Core: fix wokflow hashing for MySQL.
* Core: make `deepCopy` backward compatible.
* Editor: ensure `displayOptions` received the value from the resource locator component.
* Editor: disable the settings link in executions view for unsaved workflows.
* Editor: ensure forms reliably save.
* Editor: fix issues with interim updates in executions view.
* Editor: fix for node creator search.
* Editor: limit columns in table view to prevent the UI becoming unresponsive in the node details view.


## n8n@0.200.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.200.0...n8n@0.200.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-10-28

This is a bug fix release.

### Bug fixes

* API: do not reset the auth cookie on every request to GET `/login`.
* AWS SNS trigger node: add missing jsonParse import.
* Core: avoid callstack with circular dependencies.
* Editor: resolve issues with the executions list auto-refresh, and with saving new workflows.
* Editor: redirect the outdated `/workflow` path.
* Editor: remove a filter that prevented display of running executions.


## n8n@0.200.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.199.0...n8n@0.200.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-10-27

This release contains improvements to the editor, node enhancements and bug fixes.

### New features

* Core, editor: introduce workflow caller policy.
* Core: block workflow update on interim change.
* Editor: add a read-only state for nodes.
* Editor: add execution previews using the new **Executions** tab in the node view.
* Editor: improvements to node panel search.

### Node enhancements

* Airtable Trigger node: add the resource locator component.
* HTTP Request node: add options for raw JSON headers and queries.
* InvoiceNinja node: add support for V5.
* Write Binary File node: add option to append to a file.

### Bug fixes

* API: validate executions and workflow filter parameters.
* Core: amend typing for `jsonParse()` options.
* Core: fix `predefinedCredentialType` in node graph item.
* Core: fix canvas node execution skipping parent nodes.
* Core: fix single node execution failing in `main` mode.
* Core: set JWT authentication token `sameSite` policy to `lax`.
* Core: update to imports in helpers.
* Editor: curb item method linting in single-item mode.
* Editor: stop rendering expressions as HTML.
* Email Trigger node: backport V2 mark-seen-after processing to V1.
* Email Trigger node: improve connection handling and credentials.
* HTTP Request node: fix sending previously selected credentials.
* TheHive node: small fixes.

### Contributors


[Bram Kn](https://github.com/bramkn){:target=_blank .external-link}  
[Nicholas Penree](https://github.com/drudge){:target=_blank .external-link}  

## n8n@0.199.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.198.2...n8n@0.199.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-10-21

This release includes new nodes, an improved workflow UI, performance improvements, and bug fixes.

### New features

<div class="n8n-new-features" markdown>

#### New workflow experience

This release brings a collection of UI changes, aimed at improving the workflow experience for users. This includes:

* Removing the Start node, and adding help to guide users to find a trigger node.
* Improved node search.
* New nodes: Manual Trigger and Execute Workflow Trigger.

</div>

* Core: block workflow updates on interim changes.
* Core: enable sending client credentials in the body of API calls.
* Editor: add automatic credential selection for new nodes.

### New nodes

<div class="n8n-new-features" markdown>

#### Compare node

The Compare Datasets node helps you compare data from two input streams. You can find documentation for the new node [here](/integrations/builtin/core-nodes/n8n-nodes-base.comparedatasets/).

</div>

<div class="n8n-new-features" markdown>

#### Execute Workflow Trigger node

The Execute Workflow Trigger starts a workflow in response to another workflow. You can find documentation for the new node [here](/integrations/builtin/core-nodes/n8n-nodes-base.executeworkflowtrigger/).

</div>

<div class="n8n-new-features" markdown>

#### Manual Trigger node

The Manual Trigger allows you to start a workflow by clicking **Test Workflow**, without any option to run it automatically. You can find documentation for the new node [here](/integrations/builtin/core-nodes/n8n-nodes-base.manualworkflowtrigger/).

</div>

<div class="n8n-new-features" markdown>

#### Schedule Trigger node

This release introduces the Schedule Trigger node, replacing the Cron node. You can find documentation for the new node [here](/integrations/builtin/core-nodes/n8n-nodes-base.scheduletrigger/).

</div>

### Node enhancements

* HubSpot node: you can now use your HubSpot credentials in the HTTP Request node to make a [custom API call](/integrations/custom-operations/).
* Rundeck node: you can now use your Rundeck credentials in the HTTP Request node to make a [custom API call](/integrations/custom-operations/).

### Bug fixes

* Editor: fix a hover bug in the bottom menu.
* Editor: resolve performance issues when opening a node, or editing a code node, with a large amount of data.
* Editor: ensure workflows always stop when clicking the stop button.
* Editor: fix a bug that was causing text highlighting when mapping data in Firefox.
* Editor: ensure correct linting in the Code node editor.
* Editor: handle null values in table view.
* Elasticsearch node: fix a pagination issue.
* Google Drive node: fix typo.
* HTTP Request node: avoid errors when a response doesn't provide a content type.
* n8n node: fix a bug that was preventing the resource locator component from returning all items.

### Contributors


[AndLLA](https://github.com/AndLLA){:target=_blank .external-link}  
[Nicholas Penree](https://github.com/drudge){:target=_blank .external-link}  
[vcrwr](https://github.com/vcrwr){:target=_blank .external-link}

## n8n@0.198.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.198.1...n8n@0.198.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-10-14

This release fixes a bug affecting scrolling through parameter lists.

## n8n@0.198.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.198.0...n8n@0.198.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-10-14

This is a bug fix release.

### Bug fixes

* Editor: change the initial position of the Start node.
* Editor: align JSON view properties with their values.
* Editor: fix `BASE_PATH` for Vite dev mode.
* Editor: fix data pinning success source.

### Contributor

[Bram Kn](https://github.com/bramkn){:target=_blank .external-link}


## n8n@0.198.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.197.1...n8n@0.198.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-10-14

/// warning | Breaking changes
Please note that this version contains breaking changes to the Merge node. You can read more about them [here](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01980){:target=_blank .external-link}.
///
### New features

* Editor: update the expressions display.
* Editor: update the n8n-menu component.

### New nodes

<div class="n8n-new-features" markdown>

#### Code node

This release introduces the Code node. This node replaces both the Function and Function Item nodes. Refer to the [Code node](/integrations/builtin/core-nodes/n8n-nodes-base.code/) documentation for more information.

</div>

<div class="n8n-new-features" markdown>

#### Venafi TLS Protect Cloud trigger node

Start a workflow in response to events in your Venafi Cloud service.

</div>

### Node enhancements

* Citrix ADC node: add Certificate Install operation.
* Kafka node: add a **Use key** option for messages.
* MySQL node: use the resource locator component for table parameters, making it easier for users to browse and select their database fields from within n8n.

### Bug fixes

* Core, Editor: prevent overlap between running and pinning data.
* Core: expression evaluation of processes now respects `N8N_BLOCK_ENV_ACCESS_IN_NODE`.
* Editor: ensure the Axios base URL still works when hosted in a subfolder.
* Editor: fixes for horizontal scrollbar rendering.
* Editor: ensure the menu closes promptly when loading a credentials page.
* Editor: menu UI fixes.
* Box node: fix an issue that was causing the Create Folder operation to show extra items.
* GSuite Admin node: resolve issue that was causing the User Update operation to fail.
* GitLab trigger node: ensure this node activates reliably.
* HTTP Request node: ensure OAuth credentials work properly with predefined credentials.
* KoboToolbox node: fix the hook logs.
* SeaTable node: ensure link items show in response.
* Zoom node: resolve an issue that was causing missing output items.

### Contributors


[Jakob Backlund](https://github.com/jbacklund){:target=_blank .external-link}  
[Yan Jouanique](https://github.com/Yann-J){:target=_blank .external-link}

## n8n@0.197.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.197.0...n8n@0.197.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-10-10

This is a bug fix release. It resolves an issue with display width on the resource locator UI component.

## n8n@0.197.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.196.0...n8n@0.197.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-10-10

This release includes six new nodes, focused around infrastructure management. It also adds support for drag and drop data mapping in the JSON input view, and includes bug fixes.

### New features

* Core: improve light versioning support in declarative node design.
* Editor UI: data mapping for JSON view. You can now map data using drag and drop from JSON view, as well as table view.

### New nodes

<div class="n8n-new-features" markdown>

#### AWS Certificate Manager

A new integration with AWS Certificate Manager. You can find the documentation [here](/integrations/builtin/app-nodes/n8n-nodes-base.awscertificatemanager/).

</div>

<div class="n8n-new-features" markdown>

#### AWS Elastic Load Balancing

Manage your AWS load balancers from your workflow using the new AWS Elastic Load Balancing node. You can find the documentation [here](/integrations/builtin/app-nodes/n8n-nodes-base.awselb/).

</div>

<div class="n8n-new-features" markdown>

#### Citrix ADC

Citrix ADC is an application delivery and load balancing solution for monolithic and microservices-based applications. You can find the documentation [here](/integrations/builtin/app-nodes/n8n-nodes-base.citrixadc/).

</div>

<div class="n8n-new-features" markdown>

#### Cloudflare

Cloudflare provides a range of services to manage and protect your websites. This new node allows you to manage zone certificates in Cloudflare from your workflows. You can find the documentation [here](/integrations/builtin/app-nodes/n8n-nodes-base.cloudflare/).

</div>

<div class="n8n-new-features" markdown>

#### Venafi nodes

This release includes two new Venafi nodes, to integrate with their Protect TLS service.

</div>

### Node enhancements

Crypto node: add SHA3 support.

### Bug fixes

* CLI: cache generated assets in a user-writeable directory.
* Core: prevent excess runs when data is pinned in a trigger node.
* Core: ensure hook URLs always added correctly.
* Editor: a fix for an issue affecting linked items in combination with data pinning.
* Editor: resolve a bug with the binary data view.
* GitHub trigger node: ensure trigger executes reliably.
* Microsoft Excel node: fix pagination issue.
* Microsoft ToDo node: fix pagination issue.

### Contributors


[Stratos Theodorou](https://github.com/eeVoskos){:target=_blank .external-link}

## n8n@0.196.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.195.5...n8n@0.196.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-09-30

This release includes major new features:

* Better item linking
* New built-in variables and methods
* A redesigned main navigation
* New nodes, as well as an overhaul of the HTTP Request node

It also contains bug fixes and node enhancements.

### New features

<div class="n8n-new-features" markdown>

#### Improved item linking

Introducing improved support for item linking (paired items). Item linking is a key concept in the n8n data flow. Learn more in [Data item linking](/data/data-mapping/data-item-linking/).

</div>

<div class="n8n-new-features" markdown>

#### Overhauled built-in variables

n8n's [built-in methods and variables](/code/builtin/) have been overhauled, introducing new variables, and providing greater consistency in behavior and naming.

</div>

<div class="n8n-new-features" markdown>

#### Redesigned main navigation

We've redesigned the main navigation (the left hand menu) to create a simpler user experience.

</div>

#### Other new features

* Improved error text when loading options in a node.
* On reset, share unshared credentials with the instance owner.

### New nodes

<div class="n8n-new-features" markdown>

#### n8n node

The [n8n node](/integrations/builtin/core-nodes/n8n-nodes-base.n8n/) allows you to consume the n8n API in your workflows.

</div>

<div class="n8n-new-features" markdown>

#### WhatsApp Business Platform node

The [WhatsApp Business Platform](/integrations/builtin/app-nodes/n8n-nodes-base.whatsapp/) node allows you to use the WhatsApp Business Platform Cloud API in your workflows.

</div>

### Node enhancements

* HTTP Request node: a major overhaul. It's now much simpler to build a custom API request. Refer to the [HTTP Request node documentation](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) for more information.
* RabbitMQ trigger node: now automatically reconnects on disconnect.
* Slack node: add the 'get many' operation for users.

### Bug fixes

* Build: add typing for SSE channel.
* Build: fix lint issue.
* CLI: add git to all Docker images
* CLI: disable X-Powered-By: Express header.
* CLI: disable CORS on SSE connections in production.
* Core: remove commented out lines.
* Core: delete unused dependencies.
* Core: fix and harmonize documentation links for nodes.
* Core: remove the --forceExit flag from CLI tests.
* Editor: add missing event handler to accordion component.
* Editor: fix Storybook setup.
* Editor: ensure BASE_URL replacement works correctly on Windows.
* Editor: fix parameter input field focus.
* Editor: make lodash aliases work on case-sensitive file systems.
* Editor: fix an issue affecting copy-pasting workflows into pinned data in the code editor.
* Editor: ensure the run data pagination selector displays when appropriate.
* Editor: ensure the run selector can open.
* Editor: tidy up leftover i18n references in the node view.
* Editor: correct an i18n string.
* Editor: resolve slow loading times for node types, node creators, and push connections in the settings view.
* Nodes: update descriptions in the Merge node
* Nodes: ensure the card ID property displays for completed checklists in the Trello node.
* Nodes: fix authentication for the new verions of WeKan.
* Nodes: ensure form names list correctly in the Wufoo trigger node.

### Contributors


[Cristobal Schlaubitz Garcia](https://github.com/CxGarcia){:target=_blank .external-link}

## n8n@0.195.5

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.195.4...n8n@0.195.5){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-09-23

This is a bug fix release. It fixes an issue with extracting values in expressions.

## n8n@0.195.4

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.195.3...n8n@0.195.4){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-09-22

This release:

* Adds the ability to resize the main node panel.
* Resolves an issue with resource locator in expressions.

## n8n@0.195.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.195.2...n8n@0.195.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-09-22

This is a bug fix release.

* Editor: fix an expressions bug affecting numbers and booleans.
* Added support for setting the TDS version in Microsoft SQL credentials.

## n8n@0.195.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.195.1...n8n@0.195.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-09-22

This is a bug fix release. It resolves an issue with MySQL migrations.


## n8n@0.195.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.195.0...n8n@0.195.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-09-21

This is a bug fix release. It resolves an issue with Postgres migrations.

## n8n@0.195.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.194.0...n8n@0.195.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-09-21

This release introduces user management and credential sharing for n8n's Cloud platform. It also contains other enhancements and bug fixes.

### New features

<div class="n8n-new-features" markdown>

#### User management and credential sharing for Cloud

This release adds support for n8n's existing [user management](/user-management/) functionality to Cloud, and introduces a new feature: [credential sharing](/credentials/credential-sharing/). Credential sharing is currently only available on Cloud.

</div>

Also in this release:

* Added a `resourceLocator` parameter type for nodes, and started upgrading n8n's built-in nodes to use it. This new option helps users who need to specify the ID of a record or item in an external service. For example, when using the Trello node, you can now search for a specific card by ID, URL, or do a free text search for card titles. Node builders can learn more about working with this new UI element in n8n's [UI elements](/integrations/creating-nodes/build/reference/ui-elements/) documentation.
* Cache npm dependencies to improve performance on self-hosted n8n

### Bug fixes

* Box node: fix an issue that sometimes prevented response data from being returned.
* CLI: prevent n8n from crashing when it encounters an error in poll method.
* Core: prevent calls to constructor, to forbid arbitrary code execution.
* Editor: fix the output panel for Wait node executions.
* HTTP node: ensure instance doesn't crash when batching enabled.
* Public API: corrections to the OAuth schema.
* Xero node: fix an issue that was causing line amount types to be ignored when creating new invoices.

### Contributors


[Ikko Ashimine](https://github.com/eltociear){:target=_blank .external-link}


## n8n@0.194.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.193.5...n8n@0.194.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-09-15

This release includes new nodes: a Gmail trigger, Google Cloud Storage, and Adalo. It also contains major overhauls of the Gmail and Merge nodes.

### New features

* CLI: load all nodes and credentials code in isolation.
* Core, Editor UI: introduce support for node deprecation.
* Editor: implement HTML sanitization for Notification and Message components.
* Editor: display the input number on multi-input nodes.

### New nodes

<div class="n8n-new-features" markdown>

#### Adalo

Adalo is a low code app builder. Refer to n8n's [Adalo node documentation](/integrations/builtin/app-nodes/n8n-nodes-base.adalo/) for more information.

</div>

<div class="n8n-new-features" markdown>

#### Google Cloud Storage

n8n now has a [Google Cloud Storage node](/integrations/builtin/app-nodes/n8n-nodes-base.googlecloudstorage/). 

</div>

<div class="n8n-new-features" markdown>

#### Gmail Trigger

n8n now has a [Gmail trigger node](/integrations/builtin/trigger-nodes/n8n-nodes-base.gmailtrigger/). This allows you to trigger workflows in response to a Gmail account receiving an email.

</div>

### Node enhancements

* Gmail node: this release includes an overhaul of the [Gmail node](/integrations/builtin/app-nodes/n8n-nodes-base.gmail/), with updated resources and operations.
* Merge node: a major overhaul. Merge mode's have new names, and have been simplified. Refer to the [Merge node documentation](/integrations/builtin/core-nodes/n8n-nodes-base.merge/) to learn more.
* MongoDB node: updated the Mongo driver to 4.9.1.


### Bug fixes

* CLI: core: address Dependabot warnings.
* CLI: avoid scanning unnecessary directories on Windows.
* CLI: load nodes and directories on Windows using the correct file path.
* CLI: ensure password reset triggers internal and external hooks.
* CLI: use absolute paths for loading custom nodes and credentials.
* Core: returnJsonArray helper no longer breaks nodes that return no data.
* Core: fix an issue with node renaming and expressions.
* Core: update OAuth endpoints to use the instance base URL.
* Nodes: resolved an issue that was preventing versioned nodes from loading.
* Public API: better error handling for bad requests.
* AWS nodes: fixed an issue with credentials testing.
* GoogleBigQuery node: fix for empty responses when creating records.
* HubSpot node: correct the node name on the canvas.

### Contributors


[Rhys Williams](https://github.com/rhyswilliamsza){:target=_blank .external-link}

## n8n@0.193.5

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.193.4...n8n@0.193.5){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-09-07

This is a bug fix release.

### Bug fixes

* Editor: prevent editing in the Function nodes in executions view.
* Editor: ensure button widths are correct.
* Editor: fix a popup title.
* Gmail node: fix an issue introduced due to incorrect automatic data formatting.

## n8n@0.193.4

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.193.3...n8n@0.193.4){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-09-06

This release contains new features that lay the groundwork for upcoming releases, and bug fixes.

### New features

* It's now possible to configure the stop time for workers.
* CLI: Added external hooks for when members are added or deleted.
* Editor: Use the i18n component for localization (replacing v-html)

### Bug fixes


* CLI: include "auth-excluded" endpoints on the history middleware as well.
* Core: fix MySQL migration issue with table prefix.
* Correct spelling.
* Fix n8n-square-button import.
* AWS nodes: handle query string and body properly for AWS related requests.
* AWS Lambda node: fix JSON data being sent to AWS Lambda as string.
* Beeminder node: fix request ID not being sent when creating a new data point.
* GitHub node: fix binary data not being returned.
* GraphQL node: fix issue with return items.
* Postgres node: fix issue with Postgres insert and paired item.
* Kafka trigger node: fix Kafka trigger not working with default max requests value.
* MonicaCrm node: fix pagination when using return all.
* Gmail node: fix bug related to paired items.
* Raindrop node: fix issue refreshing OAuth2 credentials.
* Shopify node: fix pagination when empty fields are sent.

### Contributors


[Aaron Delasy](https://github.com/delasy){:target=_blank .external-link}  
[ruanjiefeng](https://github.com/ruanjf){:target=_blank .external-link}


## n8n@0.193.3

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.193.2...n8n@0.193.3){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-09-01

This release contains bug fixes and node enhancements.

### Node enhancements

MongoDB node: add credential testing and two new operations.

### Bug fixes

* CLI: only initialize the mailer if the connection can be verified.
* Core: fix an issue with disabled parent outputs in partial executions.
* Nodes: remove duplicate wrapping of paired item data.


## n8n@0.193.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.193.1...n8n@0.193.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-09-01

This is a bug fix release. It resolves an issue that was causing errors with OAuth2 credentials.

## n8n@0.193.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.193.0...n8n@0.193.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-08-31

This is a bug fix release. It resolves an issue that was preventing column headings from displaying correctly in the editor.

## n8n@0.193.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.192.2...n8n@0.193.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-08-31

This release contains a new node, feature enhancements, and bug fixes.

### New nodes

This release adds an integration for [HighLevel](/integrations/builtin/app-nodes/n8n-nodes-base.highlevel/), an all-in-one sales and marketing platform.

### Enhancements

* Docker: reduce the size of Alpine Docker images.
* Editor: improve mapping tooltip behavior.

### Bug fixes

* Core: make digest auth work with query parameters.
* Editor: send data as query on DELETE requests.
* Fix credentials_entity table migration for MySQL.
* Improve `.npmignore` to reduce the size of the published packages.

### Contributors


[pemontto](https://github.com/pemontto){:target=_blank .external-link}  
[Tzachi Shirazi](https://github.com/TzachiSh){:target=_blank .external-link}

## n8n@0.192.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.192.1...n8n@0.192.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-08-25

This is a bug fix release.

### Bug fixes

* Editor: fix the feature flag check when PostHog is unavailable.
* Editor: fix for a mapping bug that occured when value is null.

## n8n@0.192.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.192.0...n8n@0.192.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-08-25

This is a bug fix release.

### Bug fixes

Account for non-array types in `pinData` migration.

## n8n@0.192.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.191.1...n8n@0.192.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-08-24

This release contains new features and enhancements, as well as bug fixes.

### New features

<div class="n8n-new-features" markdown>

#### Map nested fields

n8n@0.187.0 saw the first release of [data mapping](/data/data-mapping/), allowing you to drag and drop top level data from a node's **INPUT** panel into parameter fields. With this release, you can now drag and drop data from any level.

</div>

* Core and editor: support `pairedItem` for pinned data.
* Core and editor: integrate PostHog.
* Core: add a command to scripts making it easier to launch n8n with tunnel.
* CLI: notify external hooks about user profile and password changes.

### Bug fixes

* Core: account for the enabled state in the first pinned trigger in a workflow.
* Core: fix pinned trigger execution.
* CLI: handle unparseable strings during JSON key migration.
* CLI: fix the excessive instantiation type error for flattened executions.
* CLI: initiate the nodes directory to ensure `npm install` succeeds.
* CLI: ensure tsc build errors also cause Turbeorepo builds to fail.
* Nextcloud node: fix an issue with credential verification.
* Freshdesk node: fix an issue where the getAll operation required non-existant options.

## n8n@0.191.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.191.0...n8n@0.191.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-08-19

This is a bug fix release. It resolves an issue that was causing node connectors to disappear after a user renamed them.

## n8n@0.191.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.190.0...n8n@0.191.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-08-17

This release lays the groundwork for wider community nodes support. It also includes some bug fixes.

### New features

* Community nodes are now enabled based on npm availability on the host system. This allows n8n to introduce community nodes to the Desktop edition in a future release.
* Improved in-app guidance on mapping data.

### Bug fixes

* CLI: fix the community node tests on Postgres and MySQL.
* Core: fix an issue preventing child workflow executions from displaying.
* Editor: handle errors when opening settings and executions.
* Editor: improve expression and parameters performance.
* Public API: fix executions pagination for n8n instances using Postgres and MySQL.

## n8n@0.190.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.189.1...n8n@0.190.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-08-10

This is a bug fix release.

### Bug fixes

* Core: fix a crash caused by parallel calls to test webhooks.
* Core: fix an issue preventing static data being saved for poll triggers.
* Public API: fix a pagination issue.
* GitHub Trigger: typo fix.

### Contributors


[Nathan Poirier](https://github.com/nathan818fr){:target=_blank .external-link}


## n8n@0.189.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.189.0...n8n@0.189.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-08-05

This is a bug fix release.

### Bug fixes

Fixed an issue with MySQL and MariaDB migrations.

## n8n@0.189.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.188.0...n8n@0.189.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-08-03

This release includes a new node, Sendinblue, as well as bug fixes.

### New nodes

[Sendinblue node](/integrations/builtin/app-nodes/n8n-nodes-base.sendinblue/) and Sendinblue trigger node: introducing n8n's [Sendinblue](https://www.sendinblue.com/){:target=_blank .external-link} integration.

### Node enhancements

[NocoDB node](/integrations/builtin/app-nodes/n8n-nodes-base.nocodb/): add support for v0.90.0+

### Bug fixes

* Editor: fix a label cut off.
* Fix an issue with saving workflows when tags are disabled.
* Ensure support for community nodes on Windows.

### Contributors


[mertmit](https://github.com/mertmit){:target=_blank .external-link}  
[Nicholas Penree](https://github.com/drudge){:target=_blank .external-link}

## n8n@0.188.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.187.2...n8n@0.188.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-07-27

This release contains a new node for Metabase, bug fixes, and node and product enhancements.

### New nodes

<div class="n8n-new-features" markdown>

#### Metabase

This release includes a new [Metabase node](/integrations/builtin/app-nodes/n8n-nodes-base.metabase/). [Metabase](https://www.metabase.com/){:target=_blank .external-link} is a business data analysis tool.

</div>

### Enhancements

This release includes improvements to n8n's core pairedItems functionality.

### Node enhancements

* [Item Lists node](/integrations/builtin/core-nodes/n8n-nodes-base.itemlists/): add an operation to create arrays from input items.
* [Kafka trigger node](/integrations/builtin/trigger-nodes/n8n-nodes-base.kafkatrigger/): add more option fields.


### Bug fixes

* Core: add Windows support to `import:credentials --separate`.
* Editor: correct linking buttons color.
* Editor: ensure data pinning works as expected when `pinData` is null.
* Editor: fix a bug with spaces.
* Editor: resolve an issue with sticky note duplication and positioning.
* Editor: restore missing header colors.
* AWS DynamoDB node: fix for errors with expression attribute names.
* Mautic node: fix an authentication issue.
* Rocketchat node: fix an authentication issue.

### Contributors


[Nicholas Penree](https://github.com/drudge){:target=_blank .external-link}

## n8n@0.187.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.187.1...n8n@0.187.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-07-21

This is a bug fix release.

* Editor: fix for a console issue.
* Editor: fix a login issue for non-admin users.
* Editor: fix problems with the credentials modal that occured when no node is open.
* NocoDB node: fix for an authentication issue.

## n8n@0.187.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.187.0...n8n@0.187.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-07-20

This release fixes a bug that was preventing new nodes from reliably displaying in all browsers.

## n8n@0.187.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.186.1...n8n@0.187.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-07-20

This release includes several major new features, including:

* The community nodes repository: a new way to build and share nodes.
* Data pinning and data mapping: accelerate workflow development with better data manipulation functionality.

### New features

<div class="n8n-new-features" markdown>

#### Community nodes repository

This release introduces the [community node repository](/integrations/community-nodes/). This allows developers to build and share nodes as npm packages. Users can install community-built nodes directly in n8n.

</div>

<div class="n8n-new-features" markdown>

#### Data pinning

[Data pinning](/data/data-pinning/) allows you to freeze and edit data during workflow development. Data pinning means saving the output data of a node, and using the saved data instead of fetching fresh data in future workflow executions. This avoids repeated API calls when developing a workflow, reducing calls to external systems, and speeding up workflow development.

</div>

<div class="n8n-new-features" markdown>

#### Data mapping

This release introduces a drag and drop interface for [data mapping](/data/data-mapping/), as a quick way to map data without using expressions.

</div>

<div class="n8n-new-features" markdown>

#### Simplify authentication setup for node creators

This release introduces a simpler way of handling authorization when building a node. All credentials should now contain an `authenticate` property that dictates how the credential is used in a request.
n8n has also simplified authentication types: instead of specifying an authentication type and using the correct interface, you can now set the type as `"generic"`, and use the `IAuthenticateGeneric` interface.

You can use this approach for any authentication method where data is sent in the header, body, or query string. This includes methods like bearer and basic auth. You can't use this approach for more complex authentication types that require multiple calls, or for methods that don't pass authentication data. This includes OAuth.

For an example of the new authentication syntax, refer to n8n's [Asana node](https://github.com/n8n-io/n8n/blob/master/packages/nodes-base/credentials/AsanaApi.credentials.ts){:target=_blank .external-link}.

```js
// in AsanaApi.credentials.ts
import {
	IAuthenticateGeneric,
	ICredentialType,
	INodeProperties,
} from 'n8n-workflow';

export class AsanaApi implements ICredentialType {
	name = 'asanaApi';
	displayName = 'Asana API';
	documentationUrl = 'asana';
	properties: INodeProperties[] = [
		{
			displayName: 'Access Token',
			name: 'accessToken',
			type: 'string',
			default: '',
		},
	];

	authenticate: IAuthenticateGeneric = {
		type: 'generic',
		properties: {
			headers: {
				Authorization: '=Bearer {{$credentials.accessToken}}',
			},
		},
	};
}
```
</div>

#### Other new features

* Added a `preAuthentication` method to credentials.
* Added more credentials tests.
* Introduce automatic fixing for paired item information in some scenarios.

### Node enhancements

* [ERPNext node](/integrations/builtin/app-nodes/n8n-nodes-base.erpnext/): add credential tests, and add support for unauthorized certs.
* [Google Drive node](/integrations/builtin/app-nodes/n8n-nodes-base.googledrive/): add support for move to trash.
* [Mindee node](/integrations/builtin/app-nodes/n8n-nodes-base.mindee/): support new version.
* [Notion node](/integrations/builtin/app-nodes/n8n-nodes-base.notion/): support ignoring the Notion URL property if empty.
* [Shopify node](/integrations/builtin/app-nodes/n8n-nodes-base.shopify/): add OAuth support.

### Bug fixes

* API: add missing node settings parameters.
* API: validate static data value for resource workflow.
* Baserow Node: fix an issue preventing table names from loading.
* Editor: hide the **Execute previous node** button when in read-only mode.
* Editor: hide tabs if there's only one branch.
* Roundup of link fixes in nodes.

### Contributors


[Florian Bachmann](https://github.com/baflo){:target=_blank .external-link}
[Olivier Aygalenq](https://github.com/oaygalenq){:target=_blank .external-link}


## n8n@0.186.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.186.0...n8n@0.186.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-07-14

This is a bug fix release. It includes a fix for an issue with the Airtable node.

## n8n@0.186.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.185.0...n8n@0.186.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-07-13

This release contains bug fixes and node enhancements.

### New features

* Add item information to more node errors.
* Update multiple credentials with tests, and add support for custom operations.

### Node enhancements


* [AWS DynamoDB node](/integrations/builtin/app-nodes/n8n-nodes-base.awsdynamodb/): improve error handling and add an optional GetAll Scan FilterExpression.
* [Customer.io node](/integrations/builtin/app-nodes/n8n-nodes-base.customerio/): add support for tracking region selection.
* [Elasticsearch node](/integrations/builtin/app-nodes/n8n-nodes-base.elasticsearch/): add 'Source Excludes' and 'Source Includes' options to the Document: getAll operation. Add credential tests, index pipelines, and index refresh.
* [Freshworks CRM node](/integrations/builtin/app-nodes/n8n-nodes-base.freshworkscrm/): add search and lookup functionality.
* [JIRA node](/integrations/builtin/trigger-nodes/n8n-nodes-base.jiratrigger/): add optional query authentication.
* [Postgres node](/integrations/builtin/app-nodes/n8n-nodes-base.postgres/): improve handling of large numbers.
* [Redis node](/integrations/builtin/app-nodes/n8n-nodes-base.redis/): add push and pop operations.
* [Rename node](/integrations/builtin/core-nodes/n8n-nodes-base.renamekeys/): add regex replace.
* [Spreadsheet file node](/integrations/builtin/core-nodes/n8n-nodes-base.spreadsheetfile/): allow skipping headers when writing spreadsheets.



### Bug fixes

* Editor: Fix an error that occured after repeated executions.
* [EmailReadImap node](/integrations/builtin/core-nodes/n8n-nodes-base.emailimap/): improve handling of network problems.
* [Google Drive node](/integrations/builtin/app-nodes/n8n-nodes-base.googledrive/): process input items using the list operation.
* [Telegram node](/integrations/builtin/app-nodes/n8n-nodes-base.telegram/): fix for a bug affecting sending binary data (images, documents and so on).

### Contributors


[Bryce Sheehan](https://github.com/ctrl-freak){:target=_blank .external-link}
[h4ux](https://github.com/h4ux){:target=_blank .external-link}
[miguel-mconf](https://github.com/miguel-mconf){:target=_blank .external-link}
[Nicholas Penree](https://github.com/drudge){:target=_blank .external-link}
[pemontto](https://github.com/pemontto){:target=_blank .external-link}
[Yann Jouanique](https://github.com/Yann-J){:target=_blank .external-link}

## n8n@0.185.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.184.0...n8n@0.185.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-07-05

This release adds a new node, Google Ads. It also contains bug fixes and node enhancements, as well as a small addition to core.

### New features

Core: add the `action` parameter to INodePropertyOptions. This parameter is now available when building nodes.

### New nodes

[Google Ads node](/integrations/builtin/app-nodes/n8n-nodes-base.googleads/): n8n now provides a Google Ads node, allowing you to get data from Google Ad campaigns.

### Node enhancements

* [DeepL node](/integrations/builtin/app-nodes/n8n-nodes-base.deepl/): Add support for longer text fields, and add credentials tests.
* [Facebook Graph API node](/integrations/builtin/app-nodes/n8n-nodes-base.facebookgraphapi/): Add support for Facebook Graph API 14.
* [JIRA node](/integrations/builtin/app-nodes/n8n-nodes-base.jira/): Add support for the simplified option with rendered fields.
* [Webflow trigger node](/integrations/builtin/trigger-nodes/n8n-nodes-base.webflowtrigger/): Reduce the chance of webhook duplication. Add a credentials test.
* [WordPress node](/integrations/builtin/app-nodes/n8n-nodes-base.wordpress/): Add a post template option.

### Bug fixes

* [HubSpot node](/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/): Fix for search endpoints.
* [KoboToolbox node](/integrations/builtin/app-nodes/n8n-nodes-base.kobotoolbox/): Improve attachment matching logic and GeoJSON Polygon format.
* [Odoo node](/integrations/builtin/app-nodes/n8n-nodes-base.odoo/): Prevent possible issues with some custom fields.
* Sticky note node: Fix an issue that was causing the main header to hide.
* [Todoist node](/integrations/builtin/app-nodes/n8n-nodes-base.todoist/): Improve multi-item support.

### Contributors


[cgobrech](https://github.com/cgobrech){:target=_blank .external-link}
[pemontto](https://github.com/pemontto){:target=_blank .external-link}
[Yann Jouanique](https://github.com/Yann-J){:target=_blank .external-link}
[Zapfmeister](https://github.com/Zapfmeister){:target=_blank .external-link}


## n8n@0.184.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.183.0...n8n@0.184.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-06-29

This release includes:

* New core features
* Enhancements to the Clockify node.
* Bug fixes.

### New features

* You can now access `getBinaryDataBuffer` in the pre-send method.
* n8n now exposes the item index being processed by a node.
* Migrated the expressions templating engine to [n8n's fork of riot-tmpl](https://github.com/n8n-io/tmpl){:target=_blank .external-link}.


### Node enhancements

[Clockify node](/integrations/builtin/app-nodes/n8n-nodes-base.clockify/): added three new resources: Client, User, and Workspace. Also added support for custom API calls.


### Bug fixes

* Core: fixed an error with logging circular links in JSON.
* Editor UI: now display the full text of long error messages.
* Editor UI: fix for an issue with credentials rendering when the node has no parameters.
* [Cortex node](/integrations/builtin/app-nodes/n8n-nodes-base.cortex/): fix an issue preventing all analyzers being returned.
* [HTTP Request node](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/): ensure all OAuth2 credentials work with this node.
* [LinkedIn node](/integrations/builtin/app-nodes/n8n-nodes-base.linkedin/): fix an issue with image preview.
* [Salesforce node](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/): fix an issue that was causing the lead status to not use the new name when name is updated.
* Fixed an issue with required/optional parameters.

### Contributors


[pemontto](https://github.com/pemontto){:target=_blank .external-link}

## n8n@0.183.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.182.1...n8n@0.183.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-06-21

This release contains node enhancements and bug fixes, as well as an improved trigger nodes panel.

### New features

Enhancements to the **Trigger** inputs panel: When using a trigger node, you will now see an **INPUT** view that gives guidance on how to load data into your trigger.

### Node enhancements

* [HubSpot node](/integrations/builtin/app-nodes/n8n-nodes-base.hubspot){:target=_blank}: you can now assign a stage on ticket update.
* [Todoist node](/integrations/builtin/app-nodes/n8n-nodes-base.todoist){:target=_blank}: it's now possible to move tasks between sections.
* [Twake node](/integrations/builtin/app-nodes/n8n-nodes-base.twake){:target=_blank}: updated icon, credential test added, and added support for custom operations.

### Bug fixes

* Core: don't allow OPTIONS requests from any source.
* Core: GET `/workflows/:id` now returns tags.
* Core: ensure predefined credentials show up in the HTTP Request node.
* Core: return the correct error message on Axios error.
* Core: updates to the expressions allow-list and deny-list.

### Contributors


[Bryce Sheehan](https://github.com/ctrl-freak){:target=_blank .external-link}
[Rahimli Rahim](https://github.com/rahimlis){:target=_blank .external-link}

## n8n@0.182.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.182.0...n8n@0.182.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-06-16

This is a bug fix release. It resolves an issue with restarting waiting executions.

## n8n@0.182.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.181.2...n8n@0.182.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-06-14

This release contains enhancements to the Twilio and Wise integrations, and adds support for a new grant type for OAuth2. It also includes some bug fixes.

### New features

Added support for the client_credentials grant type for OAuth2.

### Node enhancements

* [Twilio node](/integrations/builtin/app-nodes/n8n-nodes-base.twilio/){:target=_blank}: added the ability to make a voice call using TTS.
* [Wise node](/integrations/builtin/app-nodes/n8n-nodes-base.wise/){:target=_blank}: added support for downloading statements as JSON, CSV, or PDF.

### Bug fixes

* Core: fixes an issue that was causing parameters to get lost in some edge cases.
* Core: fixes an issue with combined expressions not resolving if one expression was invalid.
* Core: fixed an issue that was causing the public API to fail to build on Windows.
* Editor: ensure errors display correctly.
* [HTTP Request node](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/){:target=_blank}: better handling for requests that return null.
* [Pipedrive node](/integrations/builtin/app-nodes/n8n-nodes-base.pipedrive/){:target=_blank}: fixes a limits issue with the GetAll operation on the Lead resource.
* [Postbin node](/integrations/builtin/app-nodes/n8n-nodes-base.postbin/){:target=_blank}: remove a false error.

### Contributors


[Albrecht Schmidt](https://github.com/IamDrowsy){:target=_blank .external-link}
[Erick Friis](https://github.com/efriis){:target=_blank .external-link}
[JoLo](https://github.com/jolo-dev){:target=_blank .external-link}
[Shaun](https://github.com/simshaun){:target=_blank .external-link}
[Valentin Mocanu](https://github.com/rontav){:target=_blank .external-link}

## n8n@0.181.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.181.1...n8n@0.181.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-06-09

This is a bug fix release. It resolves an issue that was sometimes causing nodes to error when they didn't return data.

## n8n@0.181.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.181.0...n8n@0.181.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-06-09

This is a bug fix release. It fixes two issues with multi-input nodes.

## n8n@0.181.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.180.0...n8n@0.181.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-06-08

This release introduces the public API.

### New feature highlights

<div class="n8n-new-features" markdown>

#### The n8n public API

This release introduces the n8n public REST API. Using n8n's public API, you can programmatically perform many of the same tasks as you can in the GUI. The API includes a built-in Swagger UI playground. Refer to the [API documentation](/api/){:target=_blank} for more information.

</div>

### Other new features

* **Core**: you can now block user access to environment variables using the `N8N_BLOCK_ENV_ACCESS_IN_NODE` variable.

### Bug fixes

* **Core**: properly resolve expressions in declarative style nodes.

## n8n@0.180.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.179.0...n8n@0.180.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-06-07

This release adds a new node for Cal.com, support for tags in workflow import and export, UI improvements, node enhancements, and bug fixes.

### New features

<div class="n8n-new-features" markdown>

#### Tags in workflow import and export

When importing or exporting a workflow, the JSON can now include workflow tags.

</div>

<div class="n8n-new-features" markdown>

#### Improved handling of activation errors

n8n now supports running an error workflow in response to an activation error.

</div>

### New nodes

<div class="n8n-new-features" markdown>

#### Cal.com trigger

This release adds a new trigger node for Cal.com. Refer to the [Cal trigger documentation](/integrations/builtin/trigger-nodes/n8n-nodes-base.caltrigger/){:target=_blank} for more guidance.

</div>

### Node enhancements

* [GitHub node](/integrations/builtin/app-nodes/n8n-nodes-base.github/){:target=_blank}: add the Get All operation to the Organization resource.
* [QuickBooks node](/integrations/builtin/app-nodes/n8n-nodes-base.quickbooks/){:target=_blank}: add a new optional field for tax items.

### Bug fixes

* Restore support for `window` in expressions.
* Fix to the `user-management:reset` command.
* Resolve crashes in queue mode.
* Correct delete button hover spacing.
* Resolve a bug causing stuck loading states.
* [EmailReadImap node](/integrations/builtin/core-nodes/n8n-nodes-base.emailimap/){:target=_blank}: improve error handling.
* [HubSpot node](/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/){:target=_blank}: fix contact loading.

### Contributors


[Mark Steve Samson](https://github.com/marksteve){:target=_blank .external-link}
[Syed Ali Shahbaz](https://github.com/alishaz-polymath){:target=_blank .external-link}

## n8n@0.179.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.178.2...n8n@0.179.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-05-30

This release features a new node for PostBin, as well as various node enhancements and bug fixes.

### New nodes

<div class="n8n-new-features" markdown>

#### PostBin node

PostBin serves as a wrapper for standard HTTP libraries which can be used to test arbitrary API/Webhooks by sending requests and providing more advanced ways to analyze the responses.

</div>

### Node enhancements

* [RabbitMQ Trigger node](/integrations/builtin/trigger-nodes/n8n-nodes-base.rabbitmqtrigger/): Made message acknowledgement and parallel processing configurable.
* [ServiceNow node](/integrations/builtin/app-nodes/n8n-nodes-base.servicenow/): Added support for attachments.
* [Todoist node](/integrations/builtin/app-nodes/n8n-nodes-base.todoist/): Added support for specifying the parent task when adding and listing tasks.

### Bug fixes

* **Core**: Fixed migrations on non-public Postgres schema.
* **Core**: Mitigated possible XSS vulnerability when importing workflow templates.
* **Editor UI**: fixed erroneous hover state detection close to the sticky note button.
* **Editor UI**: fixed display behavior of credentials assigned to versioned nodes.
* [Discord node](/integrations/builtin/app-nodes/n8n-nodes-base.discord){:target=_blank}: Fixed rate limit handling.
* [Gmail node](/integrations/builtin/app-nodes/n8n-nodes-base.gmail){:target=_blank}: Fixed sending attachments in filesystem data mode.
* [Google Sheets node](/integrations/builtin/app-nodes/n8n-nodes-base.googlesheets){:target=_blank}: Fixed an error preventing the *Use Header Names as JSON Paths* option from working as expected.
* [Nextcloud node](/integrations/builtin/app-nodes/n8n-nodes-base.nextcloud){:target=_blank}: Updated the node so the list:folder operation works with Nextcloud version 24.
* [YouTube node](/integrations/builtin/app-nodes/n8n-nodes-base.youtube){:target=_blank}: Fixed problem with uploading large files.


## n8n@0.178.2

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.178.1...n8n@0.178.2){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-05-25

This is a bug fix release. It solves an issue with loading parameters when making custom operations calls.

## n8n@0.178.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.178.0...n8n@0.178.1){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-05-24

This is a bug fix release. It solves an issue with setting credentials in the HTTP Request node.

## n8n@0.178.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.177.0...n8n@0.178.0){:target=_blank .external-link} for this version.<br />
**Release date:** 2022-05-24

This release adds support for reusing existing credentials in the HTTP Request node, making it easier to do custom operation with APIs where n8n already has an integration.

The release also includes improvements to the nodes view, giving better detail about incoming data, as well as some bug fixes.

### New features

<div class="n8n-new-features" markdown>

#### Credential reuse for custom API operations

n8n supplies hundreds of nodes, allowing you to create workflows that link multiple products. However, some nodes don't include all the possible operations supported by a product's API. You can work around this by making a custom API call using the HTTP Request node.

One of the most complex parts of setting up API calls is managing authentication. To simplify this, n8n now provides a way to use existential credential types (credentials associated with n8n nodes) in the HTTP Request node.

For more information, refer to [Custom API operations](/integrations/custom-operations/){:target=_blank}.

#### Node details view

An improved node view, showing more detail about node inputs.

</div>

### Node enhancements

[Salesforce Node](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce){:target=_blank}: Add the **Country** field.

### Bug fixes

* **Editor UI**: don't display the dividing line unless necessary.
* **Editor UI**: don't display the 'Welcome' sticky in template workflows.
* [Slack Node](/integrations/builtin/app-nodes/n8n-nodes-base.slack){:target=_blank}: Fix the kick operation for the channel resource.


## n8n@0.177.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.176.0...n8n@0.177.0){:target="_blank" .external-link} for this version.<br />
**Release date:** 2022-05-17

This release contains node enhancements, an improved welcome experience, and bug fixes.

### New features

<div class="n8n-new-features" markdown>

#### Improved welcome experience

A new [introductory video](https://youtu.be/RpjQTGKm-ok){:target="_blank" .external-link}, automatically displayed for new users.

#### Automatically convert Luxon dates to strings

n8n now automatically converts Luxon DateTime objects to strings.

</div>

### Node enhancements

* [Google Drive Node](/integrations/builtin/app-nodes/n8n-nodes-base.googledrive/){:target="_blank"}: Drive upload, delete, and share operations now support shared Drives.
* [Microsoft OneDrive](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftonedrive/){:target="_blank"}: Add the rename operation for files and folders.
* [Trello](/integrations/builtin/app-nodes/n8n-nodes-base.trello/){:target="_blank"}: Add support for operations relating to board members.

### Bug fixes

* **core:** Fix call to `/executions-current` with unsaved workflow.
* **core:** Fix issue with fixedCollection having all default values.
* [Edit Image Node](/integrations/builtin/core-nodes/n8n-nodes-base.editimage/){:target="_blank"}: Fix font selection.
* [Ghost Node](/integrations/builtin/app-nodes/n8n-nodes-base.ghost/){:target="_blank"}: Fix post tags and add credential tests.
* [Google Calendar Node](/integrations/builtin/app-nodes/n8n-nodes-base.googlecalendar/){:target="_blank"}: Make it work with public calendars and clean up.
* [KoBoToolbox Node](/integrations/builtin/app-nodes/n8n-nodes-base.kobotoolbox/){:target="_blank"}: Fix query and sort + use question name in attachments.
* [Mailjet Trigger Node](/integrations/builtin/app-nodes/n8n-nodes-base.mailjet/){:target="_blank"}: Fix issue that node couldn't get activated.
* [Pipedrive Node](/integrations/builtin/app-nodes/n8n-nodes-base.pipedrive/){:target="_blank"}: Fix resolve properties when using multi option field.

### Contributors


[Cristobal Schlaubitz Garcia](https://github.com/CxGarcia){:target="_blank" .external-link}
[Yann Jouanique](https://github.com/Yann-J){:target="_blank" .external-link}

## n8n@0.176.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.175.1...n8n@0.176.0) for this version.<br />
**Release date:** 2022-05-10

This release contains bug fixes and node enhancements.

### Node enhancements

* [Pipedrive node](/integrations/builtin/app-nodes/n8n-nodes-base.pipedrive/): adds support for filters to the Organization: Get All operation.
* [Pushover node](/integrations/builtin/app-nodes/n8n-nodes-base.pushover/): adds an HTML formatting option, and a credential test.
* [UProc node](/integrations/builtin/app-nodes/n8n-nodes-base.uproc/): adds new tools.

### Bug fixes

* **core**: a fix for filtering the executions list by waiting status.
* **core**: improved webhook error messages.
* [Edit Image node](/integrations/builtin/core-nodes/n8n-nodes-base.editimage/): node now works correctly with the binary-data-mode 'filesystem'.

### Contributors


[Albert Kiskorov](https://github.com/Albatrosicks)
[Miquel Colomer](https://github.com/mcolomer)

## n8n@0.175.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.175.0...n8n@0.175.1) for this version.<br />
**Release date:** 2022-05-03

This is a bug fix release.

### Bug fixes

Fixes a bug in the editor UI related to node versioning.

## n8n@0.175.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.174.0...n8n@0.175.0) for this version.<br />
**Release date:** 2022-05-02

This release adds support for node versioning, along with node enhancements and bug fixes.



### New features

<div class="n8n-new-features" markdown>

#### Node versioning

0.175.0 adds support for a lightweight method of node versioning. One node can contain multiple versions, allowing small version increments without code duplication. To use this feature, change the `version` parameter in your node to an array, and add your version numbers, including your existing version. You can then access the version parameter with `@version` in your `displayOptions` (to control which version n8n displays). You can also query the version in your `execute` function using `const nodeVersion = this.getNode().typeVersion;`.

</div>

### Node enhancements

* [Google Sheets node](/integrations/builtin/app-nodes/n8n-nodes-base.googlesheets/): n8n now handles header names formatted as JSON paths.
* [Microsoft Dynamics CRM node](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftdynamicscrm/): add support for regions other than North America.
* [Telegram node](/integrations/builtin/app-nodes/n8n-nodes-base.telegram/): add support for querying chat administrators.

### Bug fixes

* **core**: fixed an issue that was causing n8n to apply authentication checks, even when user management was disabled.
* **core**: n8n now skips credentials checks for disabled nodes.
* **editor**: fix a bug affecting touchscreen monitors.
* [HubSpot node](/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/): fix for search operators.
* [SendGrid node](/integrations/builtin/app-nodes/n8n-nodes-base.sendgrid/): fixed an issue with sending attachments.
* [Wise node](/integrations/builtin/app-nodes/n8n-nodes-base.wise/): respect the time parameter on `get: exchangeRate`.

### Contributors


[Jack Rudenko](https://github.com/erudenko)
[MC Naveen](https://github.com/mcnaveen)
[vcrwr](https://github.com/vcrwr)


## n8n@0.174.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.173.1...n8n@0.174.0) for this version.<br />
**Release date:** 2022-04-25

### New features

<div class="n8n-new-features" markdown>

#### Sticky Notes

This release adds Sticky Notes, a new feature that allows you to annotate and comment on your workflows. Refer to the [Sticky Notes](/workflows/sticky-notes/) for more information.

</div>

### Enhancements

* **core**: allow external OAuth connection. This enhancement adds support for connecting OAuth apps without access to n8n.
* All AWS nodes now support AWS temporary credentials.
* [Google Sheets node](/integrations/builtin/app-nodes/n8n-nodes-base.googlesheets/): Added upsert support.
* [Microsoft Teams node](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftteams/): adds several enhancements:
    * An option to limit groups to "member of", rather than retrieving the whole directory.
    * An option to get all tasks from a plan instead of just a group member.
    * Autocompletion for plans, buckets, labels, and members in update fields for tasks.
* [MongoDB node](/integrations/builtin/app-nodes/n8n-nodes-base.mongodb/): you can now parse dates using dot notation.

### Bug fixes


* [Calendly trigger node](/integrations/builtin/trigger-nodes/n8n-nodes-base.calendlytrigger/): updated the logo.
* [Microsoft OneDrive node](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftonedrive/): fixed an issue that was preventing upload of files with special characters in the file name.
* [QuickBooks node](/integrations/builtin/app-nodes/n8n-nodes-base.quickbooks/): fixed a pagination issue.

### Contributors


[Basit Ali](https://github.com/BasitAli)
[Cody Stamps](https://github.com/crstamps2)
[Luiz Eduardo de Oliveira](https://github.com/luizeof)
[Oliver Trajceski](https://github.com/SchnapsterDog)
[pemontto](https://github.com/pemontto)
[Ryan Goggin](https://github.com/Goggin)


## n8n@0.173.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.173.0...n8n@0.173.1) for this version.<br />
**Release date:** 2022-04-19

Fixes a bug with the Discord node icon name.

## n8n@0.173.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.172.0...n8n@0.173.0) for this version.<br />
**Release date:** 2022-04-19

### New nodes

<div class="n8n-new-features" markdown>

#### Markdown node

[Markdown node](/integrations/builtin/core-nodes/n8n-nodes-base.markdown/): added a new Markdown node to convert between Markdown and HTML.

</div>

### Enhancements

**editor**: you can now drag and drop nodes from the nodes panel onto the canvas.

### Node enhancements

* [Discord node](/integrations/builtin/app-nodes/n8n-nodes-base.discord/): additional fields now available when sending a message to Discord.
* [GoogleBigQuery](/integrations/builtin/app-nodes/n8n-nodes-base.googlebigquery/): added support for service account authentication.
* [Google Cloud Realtime Database node](/integrations/builtin/app-nodes/n8n-nodes-base.googlecloudrealtimedatabase/): you can now select a region.
* [PagerDuty node](/integrations/builtin/app-nodes/n8n-nodes-base.pagerduty/): now supports more detail in incidents.
* [Slack node](/integrations/builtin/app-nodes/n8n-nodes-base.slack/): added support for blocks in Slack message update.

### Bug fixes

* **core**: make the email for user management case insensitive.
* **core**: add `rawBody` for XML requests.
* **editor**: fix a glitch that caused dropdowns to break after adding expressions.
* **editor**: reset text input value when closed with `Esc`.
* [Discourse node](/integrations/builtin/app-nodes/n8n-nodes-base.discourse/): fix an issue that was causing incomplete results when getting posts. Added a credentials test.
* [Zendesk trigger node](/integrations/builtin/trigger-nodes/n8n-nodes-base.zendeskTrigger): remove deprecated targets, replace with webhooks.
* [Zoho node](/integrations/builtin/app-nodes/n8n-nodes-base.zohoCrm): fix pagination issue.

### Contributors


[Florian Metz](https://github.com/Timeraa)
[Francesco Pongiluppi](https://github.com/willywongi)
[Mark Steve Samson](https://github.com/marksteve)
[Mike Quinlan](https://github.com/mjquinlan2000)


## n8n@0.172.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.171.1...n8n@0.172.0) for this version.<br />
**Release date:** 2022-04-11

### Enhancements

* Changes to the data output display in nodes.

### Node enhancements
<br>
[Magento 2 Node:](/integrations/builtin/app-nodes/n8n-nodes-base.magento2/) Added credential tests.
[PayPal Node:](/integrations/builtin/app-nodes/n8n-nodes-base.paypal/) Added credential tests and updated the API URL.

### Bug fixes

**core**: Luxon now applies the correct timezone. Refer to [Luxon](/code/luxon/) for more information.<br>
**core**: fixed an issue with localization that was preventing i18n files from loading.<br>
[Action Network Node:](/integrations/builtin/app-nodes/n8n-nodes-base.actionnetwork/) Fix a pagination issue and add credentials test.

### Contributors


[Paolo Rechia](https://github.com/paolo-rechia)

## n8n@0.171.1

View the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.171.0...n8n@0.171.1) for this version.<br />
**Release date:** 2022-04-06

This is a small bug fix release.

### Bug fixes

* **core**: fix issue with current executions not displaying.<br>
* **core**: fix an issue causing n8n to falsely skip some authentication.<br>
* [WooCommerce Node:](/integrations/builtin/app-nodes/n8n-nodes-base.wooCommerce) Fix a pagination issue with the GetAll operation.

## n8n@0.171.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.170.0...n8n@0.171.0) for this version.<br />
**Release date:** 2022-04-03

/// warning | Breaking changes
Please note that this version contains breaking changes. You can read more about them [here](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01710).
///

This release focuses on bug fixes and node enhancements, with one new feature, and one breaking change to the GraphQL node.

### Breaking change to GraphQL node

The GraphQL node now errors when the response includes an error. If you use this node, you can choose to:

* Do nothing: a GraphQL response containing an error will now cause the workflow to fail.
* Update your GraphQL node settings: set **Continue on Fail** to true to allow the workflow to continue even when the GraphQL response contains an error.

### New features

You can now download binary data from individual nodes in your workflow.

### Enhanced nodes

* [Emelia Node:](/integrations/builtin/app-nodes/n8n-nodes-base.emelia/) Add Campaign > Duplicate functionality.
* [FTP Node:](/integrations/builtin/core-nodes/n8n-nodes-base.ftp/) Add option to recursively create directories on rename.
* [Mautic Node:](/integrations/builtin/app-nodes/n8n-nodes-base.mautic/) Add credential test and allow trailing slash in host.
* [Microsoft Teams Node:](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftteams/) Add chat message support.
* [Mocean Node:](/integrations/builtin/app-nodes/n8n-nodes-base.mocean/) Add 'Delivery Report URL' option and credential tests.
* [ServiceNow Node:](/integrations/builtin/app-nodes/n8n-nodes-base.servicenow/) Add basicAuth support and fix getColumns loadOptions.
* [Strava Node:](/integrations/builtin/app-nodes/n8n-nodes-base.strava/) Add 'Get Streams' operation.


### Bug fixes

* **core:** Fix crash on webhook when last node did not return data
* [EmailReadImap Node:](/integrations/builtin/core-nodes/n8n-nodes-base.emailimap/) Fix issue that crashed process if node was configured wrong.
* [Google Tasks Node:](/integrations/builtin/app-nodes/n8n-nodes-base.googletasks/) Fix 'Show Completed' option and hide title field where not needed.
* [NocoDB Node:](/integrations/builtin/app-nodes/n8n-nodes-base.nocodb/) Fix pagination.
* [Salesforce Node:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Fix issue that 'status' did not get used for Case => Create & Update

### Contributors


* [Charles Lecalier](https://github.com/chlec)
* [d3no](https://github.com/d3no)
* [Ketan Somvanshi](https://github.com/KetanSomvanshi)
* [Luis Cipriani](https://github.com/lfcipriani)
* [pemontto](https://github.com/pemontto)
* [Rhys Williams](https://github.com/rhyswilliamsza)

## n8n@0.170.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.169.0...n8n@0.170.0) for this version.<br />
**Release date:** 2022-03-27

This release focuses on bug fixes and adding functionality to existing nodes.

### Enhanced nodes

* [Crypto Node:](/integrations/builtin/core-nodes/n8n-nodes-base.crypto/) Add Generate operation to generate random values.
* [HTTP Request Node:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Add support for OPTIONS method.
* [Jira Node:](/integrations/builtin/app-nodes/n8n-nodes-base.jira/) Add Simplify Output option to Issue > Get.
* [Reddit Node:](/integrations/builtin/app-nodes/n8n-nodes-base.reddit/) Add possibility to query saved posts.
* [Zendesk Node:](/integrations/builtin/app-nodes/n8n-nodes-base.zendesk/) Add ticket status On-hold.

### Bug fixes

* **core:** Add logs and error catches for possible failures in queue mode.<br>
* [AWS Lambda Node:](/integrations/builtin/app-nodes/n8n-nodes-base.awslambda/) Fix Invocation Type > Continue Workflow.
* [Supabase Node:](/integrations/builtin/app-nodes/n8n-nodes-base.supabase/) Send token also using Authorization Bearer; fix Row > Get operation.
* [Xero Node:](/integrations/builtin/app-nodes/n8n-nodes-base.xero/) Fix some operations and add support for setting address and phone number.
* [Wise Node:](/integrations/builtin/app-nodes/n8n-nodes-base.wise/) Fix issue when executing a transfer.

### Contributors


* [FFTDB](https://github.com/FFTDB)
* [Fred](https://github.com/choudat)
* [Jasper Zonneveld](https://github.com/JaZo)
* [pemontto](https://github.com/pemontto)
* [Sergio](https://github.com/mcmx)
* [TheFSilver](https://github.com/TheFSilver)
* [Valentin Mocanu](https://github.com/rontav)
* [Yassine Fathi](https://github.com/m4tt72)


## n8n@0.169.0

View the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.168.2...n8n@0.169.0) for this version.<br />
**Release date:** 2022-03-20

This release includes:

* New functionality for existing nodes
* A new node for Linear
* Bug fixes
* And a license change!

### New license

This release changes n8n's license, from [Apache 2.0 with Commons Clause](https://github.com/n8n-io/n8n/blob/181ba3c4e236279b65d102a8a33ae6896f160487/LICENSE.md) to [Sustainable Use License](https://github.com/n8n-io/n8n/blob/master/LICENSE.md).

This change aims to clarify n8n's license terms, and n8n's position as a fair-code project.

Read more about the new license in [License](/reference/license/).

### New nodes

* [Linear Node:](/integrations/builtin/app-nodes/n8n-nodes-base.linear/) Add Linear Node.

### Enhanced nodes

* [HTTP Request Node:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Allow Delete requests with body.
* [KoBoToolbox Node:](/integrations/builtin/app-nodes/n8n-nodes-base.kobotoolbox/) Add KoBoToolbox Regular and Trigger Node.
* [Mailjet Node:](/integrations/builtin/app-nodes/n8n-nodes-base.mailjet/) Add credential tests and support for sandbox, JSON parameters & variables.
* [Mattermost Node:](/integrations/builtin/app-nodes/n8n-nodes-base.mattermost/) Add support for Channel search.

### Other improvements

- Add support for reading IDs from file with executeBatch command.

### Bug fixes

* [GitHub node:](/integrations/builtin/app-nodes/n8n-nodes-base.github/) Fix credential tests and File List operation.
* [Telegram node:](/integrations/builtin/app-nodes/n8n-nodes-base.telegram/) Fix sending binary data when disable notification is set.

### Contributors


* [Manuel](https://github.com/tennox)
* [Marcin Kozey](https://github.com/marcinkoziej)
* [Matthew Walther](https://github.com/mashiox)
* [Yann Jouanique](https://github.com/Yann-J)

## n8n@0.168.2

For a comprehensive list of changes, view the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.168.1...n8n@0.168.2) for this version.<br />
**Release date:** 2022-03-16

This release contains an important bug fix for 0.168.0. Users on 0.168.0 or 0.168.1 should upgrade to this.

## n8n@0.168.1

For a comprehensive list of changes, view the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.168.0...n8n@0.168.1) for this version.<br />
**Release date:** 2022-03-15

A bug fix for user management: fixed an issue with email templates that was preventing owners from inviting members.

## n8n@0.168.0

For a comprehensive list of changes, view the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.167.0...n8n@0.168.0) for this version.<br />
**Release date:** 2022-03-14

### New feature: user management

User management in n8n allows you to invite people to work in your self-hosted n8n instance. It includes:

* Login and password management
* Adding and removing users
* Two account types: owner and member

Check out the [user management documentation](/user-management/) for more information.

## n8n@0.167.0

For a comprehensive list of changes, view the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.166.0...n8n@0.167.0) for this version.<br />
**Release date:** 2022-03-13

### Highlights

#### Luxon and JMESPath

0.167.0 adds support for two new libraries:

* [Luxon](https://moment.github.io/luxon/#/): a JavaScript library for working with date and time
* [JMESPath](https://jmespath.org/): a query language for JSON

You can use Luxon and JMESPath in the code editor and in expressions.

#### New expressions variables

We've added two new variables to simplify working with date and time in expressions:

* `$now`: a Luxon object containing the current timestamp. Equivalent to DateTime.now().
* `$today`: a Luxon object containing the current timestamp, rounded down to the day. Equivalent to DateTime.now().set({ hour: 0, minute: 0, second: 0, millisecond: 0 }).

#### Negative operations in If and Switch nodes

Made it easier to perform negative operations on strings.

This release adds one new operation for numbers:

* Is Not Empty

And the following new operations for strings:

* Not Ends With
* Regex Not Match
* Not Starts With
* Is Not Empty

Additionally, Regex is now labelled Regex Match.

#### New node: Redis Trigger

Added a Redis Trigger node, so you can now start workflows based on a Redis event.

* [Redis Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.redistrigger/) Added a Redis Trigger node.

### Core functionality

- Added support for [Luxon](https://moment.github.io/luxon/#/) and [JMESPath](https://jmespath.org/).
- Added two new expressions variables, `$now` and `$today`.
- Added more negative operations for numbers and strings.
- Added a link to the course from the help menu.

### Nodes


* [Facebook Graph API:](/integrations/builtin/app-nodes/n8n-nodes-base.facebookgraphapi/) Added suport for Facebook Graph API 13.
* [HubSpot:](/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/) Added suport for private app token authentication.
* [MongoDB:](/integrations/builtin/app-nodes/n8n-nodes-base.mongodb/) Added the aggregate operation.
* [Redis Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.redistrigger/) Added a Redis Trigger node.
* [Redis:](/integrations/builtin/app-nodes/n8n-nodes-base.redis/) Added support for publish operations.
* [Strapi:](/integrations/builtin/app-nodes/n8n-nodes-base.strapi/) Added support for Strapi 4.
* [WordPress:](/integrations/builtin/app-nodes/n8n-nodes-base.wordpress/) Added status as an option to getAll post requests.


### Bugfixes

- The Google Calendar node now correctly applies timezones when creating, updating, and scheduling all day events.
- Fixed a bug that occasionally caused n8n to crash, or shut down workflows unexpectedly.
- You can now use long credential type names with Postgres.

### Contributors


* [Luiz Eduardo de Oliveira Fonseca](https://github.com/luizeof)
* [Vitaliy Fratkin](https://github.com/viiy)
* [sol](https://github.com/5pecia1)
* [vcrwr](https://github.com/vcrwr)
* [FFTDB](https://github.com/FFTDB)


## n8n@0.166.0

For a comprehensive list of changes, view the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.165.1...n8n@0.166.0) for this version.<br />
**Release date:** 2022-03-08

### New nodes


* [Odoo](/integrations/builtin/app-nodes/n8n-nodes-base.odoo/)

### Enhanced nodes


* [Function:](/integrations/builtin/core-nodes/n8n-nodes-base.function/) Added support for items without a JSON key.

### Core functionality

- Added new environment variable `N8N_HIRING_BANNER_ENABLED` to enable/disable the hiring banner.
- Fixed a bug preventing keyboard shortcuts from working as expected.
- Fixed a bug causing tooltips to be hidden behind other elements.
- Fixed a bug causing some credentials to be hidden from the credentials list.

### Bug fixes


* [Baserow:](/integrations/builtin/app-nodes/n8n-nodes-base.baserow/) Fixed a bug preventing the Sorting option of the Get All operation from working as expected.
* [HTTP Request:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Fixed a bug causing Digest Authentication to fail in some scenarios.
* [Wise:](/integrations/builtin/app-nodes/n8n-nodes-base.wise/) Fixed a bug causing API requests requiring Strong Customer Authentication (SCA) to fail.

### Contributors


[pemontto](https://github.com/pemontto)

## n8n@0.165.0

For a comprehensive list of changes, view the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.164.1...n8n@0.165.0) for this version.<br />
**Release date:** 2022-02-28

/// warning | Breaking changes
Please note that this version contains breaking changes. You can read more about them [here](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01650).
///


### New nodes



* [Onfleet](/integrations/builtin/app-nodes/n8n-nodes-base.onfleet/)

### Enhanced nodes


* [Asana:](/integrations/builtin/app-nodes/n8n-nodes-base.asana/) Added Create operation to the Project resource.
* [Mautic:](/integrations/builtin/app-nodes/n8n-nodes-base.mautic/) Added Edit Contact Points, Edit Do Not Contact List, Send Email operations to Contact resource. Also added new Segment Email resource.
* [Notion (Beta):](/integrations/builtin/app-nodes/n8n-nodes-base.notion/) Added support for rollup fields to the Simplify Output option. Also added the Parent ID to the Get All operation of the Block resource.
* [Pipedrive:](/integrations/builtin/app-nodes/n8n-nodes-base.pipedrive/) Added Marketing Status field to the Create operation of the Person resource, also added User ID field to the Create and Update operations of the Person resource.

### Core functionality

- Added support for workflow templates.
- Fixed a bug causing credentials tests to fail for versioned nodes.
- Fixed a build problem by addind dependencies `@types/lodash.set` to the `workflow` package and `@types/uuid` to the `core` package.
- Fixed an error causing some resources to ignore a non-standard `N8N_PATH` value.
- Fixed an error preventing the placeholder text from being shown when entering credentials.
- Improved error handling for telemetry-related errors.

### Bug fixes


* [Orbit:](/integrations/builtin/app-nodes/n8n-nodes-base.orbit/) Fixed a bug causing API requests to use an incorrect workspace identifier.
* [TheHive:](/integrations/builtin/app-nodes/n8n-nodes-base.thehive/)  Fixed a bug causing the Ignore SSL Issues option to be applied incorrectly.

### Contributors


[alexwitkowski](https://github.com/awitkowski0), [Iñaki Breinbauer](https://github.com/quansenB), [lsemaj](https://github.com/jamesliupenn), [Luiz Eduardo de Oliveira Fonseca](https://github.com/luizeof), [Rodrigo Correia](https://github.com/rodrigoscdc), [Santiago Botero Ruiz](https://github.com/yoky-devsavant), [Saurabh Kashyap](https://github.com/saurabharch), [Ugo Bataillard](https://github.com/knshiro)

## n8n@0.164.1

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.164.0...n8n@0.164.1) for this version.<br />
**Release date:** 2022-02-20

### Core Functionality

- Fixed a bug preventing webhooks from working as expected in some scenarios.

## n8n@0.164.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.163.1...n8n@0.164.0) for this version.<br />
**Release date:** 2022-02-20

### New nodes


* [Google Chat](/integrations/builtin/app-nodes/n8n-nodes-base.googlechat/)

### Enhanced nodes


* [Grist:](/integrations/builtin/app-nodes/n8n-nodes-base.grist/) Added support for self-hosted Grist instances.
* [Telegram Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.telegramtrigger/) Added new Extra Large option to Image Size field.
* [Webhook:](/integrations/builtin/core-nodes/n8n-nodes-base.webhook/) Added new No Response Body option. Also added support for DELETE, PATCH and PUT methods.

### Core Functionality

- Added new database indices to improve the performance when querying past executions.
- Fixed a bug causing the base portion of a URL not to be prepended as expected in some scenarios.
- Fixed a bug cuasing expressions to resolve incorrectly when referencing non-existent nodes or parameters.

### Contributors


[Jhalter5Stones](https://github.com/Jhalter5Stones), [Valentina Lilova](https://github.com/valentina98), [thorstenfreitag](https://github.com/thorstenfreitag)

## n8n@0.163.1

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.163.0...n8n@0.163.1) for this version.<br />
**Release date:** 2022-02-13

### Core Functionality

- Fixed a bug preventing OAuth2 authentication from working as expected in some scenarios.

## n8n@0.163.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.162.0...n8n@0.163.0) for this version.<br />
**Release date:** 2022-02-13

### New nodes


* [HaloPSA](/integrations/builtin/app-nodes/n8n-nodes-base.halopsa/)
* [Linear Trigger](/integrations/builtin/trigger-nodes/n8n-nodes-base.lineartrigger/)
* [Zammad](/integrations/builtin/app-nodes/n8n-nodes-base.zammad/)

### Enhanced nodes


* [GitHub:](/integrations/builtin/app-nodes/n8n-nodes-base.github/) Added Reference option to the Get operation of the File resource.
* [Twilio:](/integrations/builtin/app-nodes/n8n-nodes-base.twilio/) Added Status Callbacks option.
* [uProc:](/integrations/builtin/app-nodes/n8n-nodes-base.uproc/) Sanitized Data Webhook field description.

### Core Functionality

- Added automatic sorting by relative position to the node list inside the expression editor.
- Added new `/workflows/demo` page to allow read-only rendering of workflows inside an iframe.
- Added optional `/healthz` health check endpoint to worker instances.
- Fixed unwanted list autofill behaviour inside the expression editor.
- Improved the GitHub actions used by the nightly Docker image.

### Bug fixes


* [Function:](/integrations/builtin/core-nodes/n8n-nodes-base.function/) Fixed a bug leaving the code editor size unchanged after resizing the window.
* [Function Item:](/integrations/builtin/core-nodes/n8n-nodes-base.functionitem/) Fixed a bug leaving the code editor size unchanged after resizing the window.
* [IF:](/integrations/builtin/core-nodes/n8n-nodes-base.if/) Removed the empty sections left after removing a condition.
* [Item Lists:](/integrations/builtin/core-nodes/n8n-nodes-base.itemlists/) Fixed an erroneous placeholder text.

### Contributors


[Iñaki Breinbauer](https://github.com/quansenB), [Manuel](https://github.com/tennox), [pemontto](https://github.com/pemontto)

## n8n@0.162.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.161.1...n8n@0.162.0) for this version.<br />
**Release date:** 2022-02-06

### Enhanced nodes


* [GitHub:](/integrations/builtin/app-nodes/n8n-nodes-base.github/) Added new List operation to File resource.

### Core Functionality

- Added configurable debug logging for telemetry.
- Added support for defining nodes through JSON. This functionality is in alpha state and breaking changes to the interface can take place in upcoming versions.
- Added telemetry support to page events occuring before telemetry is initialized.
- Fixed a bug preventing errors in sub-workflows from appearing in parent executions.
- Fixed a bug where node versioning would not work as expected.
- Fixed a bug where remote parameters would not load as expected.
- Fixed a bug where unkown node types would not work as expected.
- Prevented the node details view from opening automatically after duplicating a node.
- Removed dependency `fibers` which is incompatible with the current LTS version 16 of Node.js.

### Bug fixes


* [XML:](/integrations/builtin/core-nodes/n8n-nodes-base.xml/) Fixed a bug causing the node to alter incoming data.

### Contributors


[pemontto](https://github.com/pemontto)

## n8n@0.161.1

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.161.0...n8n@0.161.1) for this version.<br />
**Release date:** 2022-02-01

### Core Functionality

- Added optional debug logging to health check functionality.

## n8n@0.161.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.160.0...n8n@0.161.0) for this version.<br />
**Release date:** 2022-01-30

### Core Functionality

- Added default polling interval for trigger nodes using polling.
- Added support for additional hints below parameter fields.
- Fixed a bug preventing default values from being used when testing credentials.
- Improved the wording in the *Save your Changes?* dialog.

### Bug fixes


* [Airtable:](/integrations/builtin/app-nodes/n8n-nodes-base.airtable/) Improved field description.
* [Airtable Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.airtabletrigger/) Improved field description.
* [erpNext:](/integrations/builtin/app-nodes/n8n-nodes-base.erpnext/) Prevented the node from throwing an error when no data is found.
* [Gmail:](/integrations/builtin/app-nodes/n8n-nodes-base.gmail/) Fixed a bug causing the BCC field to be ignored.
* [Move Binary Data:](/integrations/builtin/core-nodes/n8n-nodes-base.movebinarydata/) Fixed a bug causing the binary data to JSON conversion to fail when using filesystem-based binary data handling.
* [Slack:](/integrations/builtin/app-nodes/n8n-nodes-base.slack/) Fixed a typo in the Type field.

### Contributors


[fabian wohlgemuth](https://github.com/wohfab)

## n8n@0.160.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.159.1...n8n@0.160.0) for this version.<br />
**Release date:** 2022-01-22

### New nodes


* [BambooHR](/integrations/builtin/app-nodes/n8n-nodes-base.bamboohr/)

### Core Functionality

- Fixed a bug preventing the binary data preview from using the full available height and width.
- Fixed a build problem by pinning chokidar version 3.5.2.
- Prevent workflow activation when no trigger is presentand introduced a modal explaining production data handling.
- Fixed *Filter by tags* placeholder text used in the Open Workflow modal.

### Bug fixes


* [HTTP Request:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Fixed a bug causing custom headers from being ignored.
* [Mautic:](/integrations/builtin/app-nodes/n8n-nodes-base.mautic/) Fixed a bug preventing all items from being returned in some situations.
* [Microsoft OneDrive:](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftonedrive/) Fixed a bug preventing more than 200 items from being returned.
* [Spotify:](/integrations/builtin/app-nodes/n8n-nodes-base.spotify/) Fixed a bug causing the execution to fail if there are more than 1000 search results, also fixed a bug preventing the Get New Releases operation of the Album resource from working as expected.

### Contributors


[fabian wohlgemuth](https://github.com/wohfab)

## n8n@0.159.1

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.159.0...n8n@0.159.1) for this version.<br />
**Release date:** 2022-01-18

### Core Functionality

- Temporarily removed debug logging for Axios requests.

## n8n@0.159.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.158.0...n8n@0.159.0) for this version.<br />
**Release date:** 2022-01-16

### New nodes


* [Jenkins](/integrations/builtin/app-nodes/n8n-nodes-base.jenkins/)

### Enhanced nodes


* [GraphQL:](/integrations/builtin/core-nodes/n8n-nodes-base.graphql/) Added support for additional authentication methods Basic Auth, Digest Auth, OAuth1, OAuth2, and Query Auth.

### Core Functionality

- Added support for executing workflows without an ID through the CLI.
- Fixed a build problem.
- Fixed a bug preventing the tag description from being shown on the canvas.
- Improved build performance by skipping the `node-dev` package during build.

### Bug fixes


* [Box:](/integrations/builtin/app-nodes/n8n-nodes-base.box/) Fixed a bug causing some files to be corrupted during download.
* [Philips Hue:](/integrations/builtin/app-nodes/n8n-nodes-base.philipshue/) Fixed a bug preventing the node from connecting to Philips Hue.
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Fixed a bug preventing filters on date and datetime fields from working as expected.
* [Supabase:](/integrations/builtin/app-nodes/n8n-nodes-base.supabase/) Fixed an errorneous documentation link.

### Contributors


[Phil Clifford](https://github.com/philclifford)

## n8n@0.158.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.157.1...n8n@0.158.0) for this version.<br />
**Release date:** 2022-01-09

### New nodes


* [Microsoft Graph Security](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftgraphsecurity/)
* [SyncroMSP](/integrations/builtin/app-nodes/n8n-nodes-base.syncromsp/)
* [Supabase](/integrations/builtin/app-nodes/n8n-nodes-base.supabase/)

### Enhanced nodes


* [Edit Image:](/integrations/builtin/core-nodes/n8n-nodes-base.editimage/) Added Transparent operation.
* [Kafka:](/integrations/builtin/app-nodes/n8n-nodes-base.kafka/) Added Use Schema Registry option.
* [Kafka Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.kafkatrigger/) Added Use Schema Registry option.
* [Redis:](/integrations/builtin/app-nodes/n8n-nodes-base.redis/) Added database field to credentials.
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Added Account Number field.

### Core Functionality

- Added new external hook when active workflows finished initializing.
- Fixed a bug preventing the personalisation survey from showing up.
- Improved telemetry.

### Bug fixes


* [Edit Image:](/integrations/builtin/core-nodes/n8n-nodes-base.editimage/) Fixed a bug causing two items to be returned.
* [iCalendar:](/integrations/builtin/core-nodes/n8n-nodes-base.ical/) Fixed a bug preventing dates in January from working as expected.
* [Merge:](/integrations/builtin/core-nodes/n8n-nodes-base.merge/) Fixed causing empty binary data to overwrite other binary data on merge.

### Contributors


[Ricardo Georgel](https://github.com/rgeorgel), [Pierre](https://github.com/hnb2), [Vahid Sebto](https://github.com/sebto)

## n8n@0.157.1

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.157.0...n8n@0.157.1) for this version.<br />
**Release date:** 2022-01-03

### Core Functionality

- Fixed a bug where not all nodes could use the new binary data handling.

## n8n@0.157.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.156.0...n8n@0.157.0) for this version.<br />
**Release date:** 2022-01-02

### Enhanced nodes


* [Function:](/integrations/builtin/core-nodes/n8n-nodes-base.function/) The node now prevents unsupported data from being returned.
* [Function Item:](/integrations/builtin/core-nodes/n8n-nodes-base.functionitem/) The node now prevents unsupported data from being returned.
* [HubSpot:](/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/) Added Engagement resource with Create, Delete, Get, and Get All operations.
* [Notion (Beta):](/integrations/builtin/app-nodes/n8n-nodes-base.notion/) Upgraded the Notion node: Added Search operation for the Database resource, Get operation for Database Page resource, Archive operation for the Page resource. Also added Simplify Output option and test for credential validity.
* [Wait:](/integrations/builtin/core-nodes/n8n-nodes-base.wait/) Added new Ignore Bots option.
* [Webhook:](/integrations/builtin/core-nodes/n8n-nodes-base.webhook/) Added new Ignore Bots option.

### Core Functionality

- Fixed a bug where a wrong number suffix was used after duplicating nodes.

### Bug fixes


* [HTTP Request:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Fixed a bug where using Digest Auth would fail.

### Contributors


[pemontto](https://github.com/pemontto)

## n8n@0.156.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.155.2...n8n@0.156.0) for this version.<br />
**Release date:** 2021-12-25

### Enhanced nodes


* [GitLab Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.gitlabtrigger/) Added new trigger events: Confidential Issue, Confidential Comment, Deployment, Release.
* [Google Drive:](/integrations/builtin/app-nodes/n8n-nodes-base.googledrive/) Added support for downloading and converting native Google files.
* [Kitemaker:](/integrations/builtin/app-nodes/n8n-nodes-base.kitemaker/) Added Space ID field to Create operation of Work Item resource.
* [Raindrop:](/integrations/builtin/app-nodes/n8n-nodes-base.raindrop/) Added Parse Metadata option to Create, Update operations of the Bookmark resource.

### Core Functionality

- Added execution ID to workflow.postExecute hook
- Added response body to UI for failed Axios requests
- Added support for automatically removing new lines from Google Service Account credentials
- Added support for disabling the UI using environment variable
- Fixed a bug causing the wrong expression result to be shown for items from an output other than the first
- Improved binary data management
- Introduced Monaco as new UI code editor

### Contributors


[Arpad Gabor](https://github.com/arpadgabor), [Leo Lou](https://github.com/l4u), [Manuel](https://github.com/tennox)

## n8n@0.155.2

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.154.0...n8n@0.155.2) for this version.<br />
**Release date:** 2021-12-19

### Core Functionality

- Added support for internationalization (i18n). This functionality is currently in alpha status and breaking changes are to be expected.

## n8n@0.154.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.153.0...n8n@0.154.0) for this version.<br />
**Release date:** 2021-12-19

### Enhanced nodes


* [Plivo:](/integrations/builtin/app-nodes/n8n-nodes-base.plivo/) Added user agent to all API requests.

### Core Functionality

- Allow deletion of nodes from the canvas using the backspace key
- Fixed an issue causing clicks in the value survey to impact the main view
- Fixed an issue preventing the update panel from closing

### Bug fixes


* [Todoist:](/integrations/builtin/app-nodes/n8n-nodes-base.todoist/) Fixed a bug where using the additional field Due Date Time on the Task resource would cause the Create operation to fail.

### Contributors


[Mohammed Huzaif](https://github.com/huzaif-plivo), [Лебедев Иван](https://github.com/X-pech)

## n8n@0.153.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.152.0...n8n@0.153.0) for this version.<br />
**Release date:** 2021-12-11

### New nodes


* [Figma Trigger (Beta)](/integrations/builtin/trigger-nodes/n8n-nodes-base.figmatrigger/)
* [Workable Trigger](/integrations/builtin/trigger-nodes/n8n-nodes-base.workabletrigger/)

### Enhanced nodes


* [Google Contacts:](/integrations/builtin/app-nodes/n8n-nodes-base.googlecontacts/) Added Query option to Get All operation, also prevented the node from failing when no contacts are found.
* [HTTP Request:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Added support for query-based authentication.
* [Home Assistant:](/integrations/builtin/app-nodes/n8n-nodes-base.homeassistant/) Added support for loading possible options in the Domain, Service, and Entity ID fields.
* [One Simple API:](/integrations/builtin/app-nodes/n8n-nodes-base.onesimpleapi/) Added support for Social Profile resources.
* [PagerDuty:](/integrations/builtin/app-nodes/n8n-nodes-base.pagerduty/) Write scope is now requested upon authentication against the PagerDuty OAuth2 API.

### Core Functionality

- Added frontend for value surveys
- Fixed an issue preventing the recommendation logic from working as expected after selecting a work area
- Fixed an issue where a wrong exit code was sent when running n8n on an unsupported version of Node.js
- Fixed an issue where node options would disappear on hovering when a node isn't selected
- Fixed an issue where the execution id was missing when running n8n in queue mode
- Fixed an issue where execution data was missing when waiting for a webhook in queue mode
- Improved error handling when the n8n port is already in use
- Improved diagnostic events
- Removed toast notification on webhook deletion, added toast notification after node is copied
- Removed default trigger tooltip for polling trigger nodes

### Bug fixes


* [APITemplate.io:](/integrations/builtin/app-nodes/n8n-nodes-base.apitemplateio/) Fixed a bug where the Create operation on the Image resource would fail when the Download option isn't enabled.
* [HubSpot:](/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/) Fixed authentication for new HubSpot applications by using granular scopes when authenticating against the HubSpot OAuth2 API.
* [HubSpot Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.hubspottrigger/) Fixed authentication for new HubSpot applications by using granular scopes when authenticating against the HubSpot Developer API.
* [Jira Software:](/integrations/builtin/app-nodes/n8n-nodes-base.jira/) Fixed an issue where the Reporter field would not work as expected on Jira Server instances.
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Fixed a typo preventing the value in the amount field of from being saved.

### Contributors


[pemontto](https://github.com/pemontto), [Jascha Lülsdorf](https://github.com/buelsenfrucht), [Jonathan Bennetts](https://github.com/Joffcom)

## n8n@0.152.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.151.0...n8n@0.152.0) for this version.<br />
**Release date:** 2021-12-04

### New nodes


* [Google Calendar Trigger](/integrations/builtin/trigger-nodes/n8n-nodes-base.googlecalendartrigger/)

### Enhanced nodes


* [Telegram Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.telegramtrigger/) Added support for downloading images to channel_post updates.

### Core Functionality

- Added a plus (+) connector to end nodes
- Allowed opening workflows and executions in a new window when using Ctrl + Click
- Enforced type checking for all node parameters
- Fixed a build issue in the custom n8n docker image
- Fixed a memory leak in the UI which could occur when renaming nodes or navigate to another workflow
- Improved stability of internal test workflows
- Improved expression security
- Introduced redirect to a new page and UI error message when trying to open a deleted workflow
- Introduced support for multiple arguments when logging
- Updated the onboarding survey

### Bug fixes


* [Google BigQuery:](/integrations/builtin/app-nodes/n8n-nodes-base.googlebigquery/) Fixed a bug preventing pagination from working as expected when the Return All option is enabled.
* [RabbitMQ Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.rabbitmqtrigger/) Added Trigger to the name of the trigger node.
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Fixed a typo affecting the Type field of the Opportunity resource.

### Contributors


[Zvonimir Erdelja](https://github.com/zvonimir-ebot7), [m2scared](https://github.com/m2scared)

## n8n@0.151.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.150.0...n8n@0.151.0) for this version.<br />
**Release date:** 2021-11-26

### New nodes


* [DHL](/integrations/builtin/app-nodes/n8n-nodes-base.dhl/)
* [Grafana](/integrations/builtin/app-nodes/n8n-nodes-base.grafana/)

### Core Functionality

- Fixed a bug causing connections between nodes to disappear when renaming a newly added node after drawing a connection to its endpoints.
- Fixed a build issue by adding TypeScript definitions for validator.js to CLI package, also fixed a linting issue by removing an unused import.
- Improved the waiting state of trigger nodes to explain when an external event is required.
- Loops are now drawn below their source node.

### Bug fixes


* [Edit Image:](/integrations/builtin/core-nodes/n8n-nodes-base.editimage/) Fixed an issue preventing the Composite operation from working correctly in some cases.

### Contributors


[Jonathan Bennetts](https://github.com/Joffcom)

## n8n@0.150.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.149.0...n8n@0.150.0) for this version.<br />
**Release date:** 2021-11-19

### Enhanced nodes


* [Jira Software:](/integrations/builtin/app-nodes/n8n-nodes-base.jira/) Added Components as an additional field.

### Core Functionality

- Fixed a build issue by pinning rudder-sdk-node version 1.0.6 in CLI package.
- Fixed an issue preventing the `n8n import:workflow --separate` CLI command from finding workflows on Windows.
- Further improved the expression security.
- Moved all nodes into separate directories in preparation for internationalization.
- Removing default headers for PUT and PATCH operations when using Axios.
- Revamped the workflow canvas.

### Bug fixes


* [HTTP Request:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Fixed an issue causing the wrong Content-Type header to be set when downloading a file.
* [ServiceNow:](/integrations/builtin/app-nodes/n8n-nodes-base.servicenow/) Fixed incorrect mapping of incident urgency and impact values.
* [Start:](/integrations/builtin/core-nodes/n8n-nodes-base.start/) Fixed an issue causing the node to be disabled in a new workflow.
* [Xero:](/integrations/builtin/app-nodes/n8n-nodes-base.xero/) Fixed an issue causing the node to only fetch the first page when querying the Xero API.

## n8n@0.149.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.148.0...n8n@0.149.0) for this version.<br />
**Release date:** 2021-11-13

### New nodes


* [One Simple API](/integrations/builtin/app-nodes/n8n-nodes-base.onesimpleapi/)

### Enhanced nodes


* [Edit Image:](/integrations/builtin/core-nodes/n8n-nodes-base.editimage/) Added Circle Primitive to Draw operation. Also added Composite operation.
* [Zendesk:](/integrations/builtin/app-nodes/n8n-nodes-base.zendesk/) Added check for API credentials validity.
* [Zulip:](/integrations/builtin/app-nodes/n8n-nodes-base.zulip/) Added additional field Role to the Update operation of the User resource.

### Core Functionality

- Fixed an issue causing an error message to be thrown when executing a workflow through the CLI.
- Improved expression security by limiting the available process properties.
- Improved the behaviour of internal tests executed through the CLI.
- Updated the owner of the node user's home directory in the custom docker image.

### Bug fixes


* [Google Tasks:](/integrations/builtin/app-nodes/n8n-nodes-base.googletasks/) Fixed an issue where the Due Date field had no effect (Update operation) or was unavailable (Create operation).
* [HTTP Request:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Fixed an issue where the Content-Length header was not calculated and sent when using the a Body Content Type of Form-Data Multipart.
* [Stripe Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.stripetrigger/) Fixed an issue preventing the node from being activated when a previously created webhook no longer exists.
* [Toggl Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.toggltrigger/) Updated the API URL used by the node.

### Contributors


[GeylaniBerk](https://github.com/GeylaniBerk), [Jonathan Bennetts](https://github.com/Joffcom)

## n8n@0.148.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.147.1...n8n@0.148.0) for this version.<br />
**Release date:** 2021-11-05

### New nodes


* [Dropcontact](/integrations/builtin/app-nodes/n8n-nodes-base.dropcontact/)
* [Respond to Webhook](/integrations/builtin/core-nodes/n8n-nodes-base.respondtowebhook/)

### Enhanced nodes


* [Lemlist:](/integrations/builtin/app-nodes/n8n-nodes-base.lemlist/) Added additional fields to Create operation of Lead resource.
* [Slack:](/integrations/builtin/app-nodes/n8n-nodes-base.slack/) Added User Group resource.
* [Todoist:](/integrations/builtin/app-nodes/n8n-nodes-base.todoist/) Added Update operation to Task resource.
* [Wait:](/integrations/builtin/core-nodes/n8n-nodes-base.wait/) Improved descriptions of available Respond options.
* [WooCommerce:](/integrations/builtin/app-nodes/n8n-nodes-base.woocommerce/) Added password field to Crate operation of Customer resource.

### Core Functionality

- Added a hook after workflow creation.
- Fixed a build issue with npm v7 by overriding unwanted behaviour through the .npmrc file.
- Fixed an issue preventing unknown node types from being imported.
- Fixed an issue with the UI falsely indicating a credential can't be selected when using SQLite and multiple credentials with the same name exist.

### Bug fixes


* [Stripe:](/integrations/builtin/app-nodes/n8n-nodes-base.stripe/) Fixed an issue where setting additional Metadata fields would not have the expected effect. Also fixed an issue where pagination would not work as expected.
* [Zendesk:](/integrations/builtin/app-nodes/n8n-nodes-base.zendesk/) Fixed an issue preventing the additional field External ID from being evaulated correctly.

### Contributors


[mizzimizzi](https://github.com/mizzimizzi), [nikozila](https://github.com/nikozila), [Pauline](https://github.com/PaulineDropcontact)

## n8n@0.147.1

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.147.0...n8n@0.147.1) for this version.<br />
**Release date:** 2021-11-03

### Core Functionality

- Fixed a build issue by moving the `chokidar` dependency to a regular dependency.

## n8n@0.147.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.146.0...n8n@0.147.0) for this version.<br />
**Release date:** 2021-11-03

### New nodes


* [Local File Trigger](/integrations/builtin/core-nodes/n8n-nodes-base.localfiletrigger/)

### Core Functionality

- Improved the database migration process to reduce memory footprint.
- Fixed an issue with telemetry by adding an anonymous ID.

## n8n@0.146.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.145.0...n8n@0.146.0) for this version.<br />
**Release date:** 2021-10-29

### New nodes


* [Microsoft Dynamics CRM](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftdynamicscrm/)

### Enhanced nodes


* [Agile CRM:](/integrations/builtin/app-nodes/n8n-nodes-base.agilecrm/) Added Filters to Get All operation of Contact and Company resources.
* [Date & Time:](/integrations/builtin/core-nodes/n8n-nodes-base.datetime/) Ensuring the return values are always of type string.
* [IF:](/integrations/builtin/core-nodes/n8n-nodes-base.if/) Added support for moment types to Date & Time condition.

### Core Functionality

- Added name and ID of a workflow to its settings.
- Added parameter inputs to be multi-line.
- Fixed an issue with declaring proxies when Axios is used.
- Fixed an issue with serializing arrays and special characters.
- Fixed an issue with updating expressions after renaming a node.

### Bug fixes


* [HTTP Request:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Fixed an issue with the Full Response option not taking effect when used with the Ignore Response Code option.

### Contributors


[Valentina Lilova](https://github.com/valentina98), [Oliver Trajceski](https://github.com/SchnapsterDog)

## n8n@0.145.0

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.144.0...n8n@0.145.0) for this version.<br />
**Release date:** 2021-10-22

### New nodes


* [AWS Textract](/integrations/builtin/app-nodes/n8n-nodes-base.awstextract/)
* [Google Drive Trigger](/integrations/builtin/trigger-nodes/n8n-nodes-base.googledrivetrigger/)

### Enhanced nodes


* [Bitbucket Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.bitbuckettrigger/) Added check for credentials validity. Removed deprecated User and Team resources, and added the Workspace resource.
* [GitHub:](/integrations/builtin/app-nodes/n8n-nodes-base.github/) Added check for API credentials validity.
* [Home Assistant:](/integrations/builtin/app-nodes/n8n-nodes-base.homeassistant/) Added check for credentials validity.
* [Jira Software:](/integrations/builtin/app-nodes/n8n-nodes-base.jira/) Added check for credentials validity.
* [Microsoft OneDrive:](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftonedrive/) Added functionality to create folder hierarchy automatically upon subfolder creation.
* [Pipedrive:](/integrations/builtin/app-nodes/n8n-nodes-base.pipedrive/) Added All Users option to Get All operation of Activity resource.
* [Slack:](/integrations/builtin/app-nodes/n8n-nodes-base.slack/) Increase the Slack default query limit from 5 to 100 in order to reduce number of requests.
* [Twitter:](/integrations/builtin/app-nodes/n8n-nodes-base.twitter/) Added Tweet Mode additional field to the Search operation of Tweet resource.

### Core Functionality

- Changed `vm2` library version from `3.9.3` to `3.9.5`.
- Fixed an issue with ignoring the response code.
- Fixed an issue with overwriting credentials using environment variables.
- Fixed an issue with using query strings combined with the `x-www-form-urlencoded` content type.
- Introduced telemetry.

### Bug fixes


* [Jira Software:](/integrations/builtin/app-nodes/n8n-nodes-base.jira/) Fixed an issue with the Expand option for the Issue resource. Also fixed an issue with using custom fields on Jira Server.
* [Slack:](/integrations/builtin/app-nodes/n8n-nodes-base.slack/) Fixed an issue with pagination when loading more than 1,000 channels.
* [Strapi:](/integrations/builtin/app-nodes/n8n-nodes-base.strapi/) Fixed an issue using the Where option of the Get All operation.
* [WooCommerce:](/integrations/builtin/app-nodes/n8n-nodes-base.woocommerce/) Fixed an issue where a wrong postcode field name was used for the Order resource.

### Contributors


[pemontto](https://github.com/pemontto), [rdd2](https://github.com/rdd2), [robertodamiani](https://github.com/robertodamiani), [Rodrigo Correia](https://github.com/rodrigoscdc)

## n8n@0.144.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.143.0...n8n@0.144.0) for this version.<br />
**Release date:** 2021-10-15

### Enhanced nodes

* [Nextcloud:](/integrations/builtin/app-nodes/n8n-nodes-base.nextcloud/) Added Share operation to the File and Folder resources.
* [Zendesk:](/integrations/builtin/app-nodes/n8n-nodes-base.zendesk/) Added support for deleting, listing, getting, and recovering suspended tickets. Added the query option for regular tickets. Added assignee emails, internal notes, and public replies options to the update ticket operation.

### Core Functionality
- Improved the autofill behaviour on Google Chrome when entering credentials.

### Bug fixes

* [Airtable:](/integrations/builtin/app-nodes/n8n-nodes-base.airtable/) Fixed an issue with the sort field.
* [Cron:](/integrations/builtin/core-nodes/n8n-nodes-base.cron/) Set the version of the cron library to 1.7.2.

### Contributors

[Jonathan Bennetts](https://github.com/Joffcom)

## n8n@0.143.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.142.0...n8n@0.143.0) for this version.<br />
**Release date:** 2021-10-14

### Enhanced nodes

* [Pipedrive:](/integrations/builtin/app-nodes/n8n-nodes-base.pipedrive/) Added support for getting activities from deal ID.
* [Facebook Graph API:](/integrations/builtin/app-nodes/n8n-nodes-base.facebookgraphapi/) Added support for Facebook Graph API versions 11 and 12.

### Core Functionality
- Fixed a build issue affecting a number of AWS nodes.
- Changed workflows to use credential ids primarily (instead of names), allowing users to have different credentials with the same name.

### Bug fixes

* [ FTP:](/integrations/builtin/core-nodes/n8n-nodes-base.ftp/) Fixed error when opening FTP/SFTP credentials.

### Contributors

[Rodrigo Correia](https://github.com/rodrigoscdc)

## n8n@0.142.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.141.1...n8n@0.142.0) for this version.<br />
**Release date:** 2021-10-07

### New nodes

* [Stop and Error](/integrations/builtin/core-nodes/n8n-nodes-base.stopanderror/)

### Core Functionality
- Fixed overlapping buttons when viewing on mobile.
- Fixed issue with partial workflow executions when Wait node was last.
- Fixed issue with broken non-JSON requests.
- Node errors now only displayed for executing nodes, not disconnected nodes.
- Automatic save when executing new workflows with Webhook node.
- Fixed an issue with how arrays were serialized for certain nodes.
- Fixed an issue where executions could not be cancelled when running in Main mode.
- Duplicated workflows now open in a new window.

### Bug fixes

* [HTTP Request:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Fixed 'Ignore response code' flag.
* [Rundeck:](/integrations/builtin/app-nodes/n8n-nodes-base.rundeck/) Fixed issue with async loading of credentials.
* [SeaTable:](/integrations/builtin/app-nodes/n8n-nodes-base.seatable/) Fixed issue when entering a Baser URI with a trailing slash.

### Contributors

[Günther](https://github.com/erbg), [Tom Klingenberg](https://github.com/ktomk)

## n8n@0.141.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.141.0...n8n@0.141.1) for this version.<br />
**Release date:** 2021-10-01

### Core Functionality
- Fixed issue with body formatting of `x-form-www-urlencoded` requests.

## n8n@0.141.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.140.0...n8n@0.141.0) for this version.<br />
**Release date:** 2021-09-30

### New nodes

* [Grist](/integrations/builtin/app-nodes/n8n-nodes-base.grist/)
* [SeaTable](/integrations/builtin/app-nodes/n8n-nodes-base.seatable/)
* [SeaTable Trigger](/integrations/builtin/trigger-nodes/n8n-nodes-base.seatabletrigger/)
* [urlscan.io](/integrations/builtin/app-nodes/n8n-nodes-base.urlscanio/)

### Core Functionality
- Performance improvements in Editor UI
- Improved error reporting

### Contributors

[Alex Hall](https://github.com/alexmojaki), [Tom Klingenberg](https://github.com/ktomk)

## n8n@0.140.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.139.1...n8n@0.140.0) for this version.<br />
**Release date:** 2021-09-29

### New nodes

* [Splunk](/integrations/builtin/app-nodes/n8n-nodes-base.splunk/)

### Enhanced nodes

* [Telegram:](/integrations/builtin/app-nodes/n8n-nodes-base.telegram/) Added binary data support to the Send Animation, Send Audio, Send Document, Send Photo, Send Video, and Send Sticker operations.

### Core Functionality
- Fixed startup behavior when running n8n in scaled mode (i.e. `skipWebhoooksDeregistrationOnShutdown` is enabled).
- Fixed behavior around handling empty response bodies.
- Fixed an issue with handling of refresh tokens.

### Contributors

[pemontto](https://github.com/pemontto)

## n8n@0.139.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.139.0...n8n@0.139.1) for this version.<br />
**Release date:** 2021-09-23

### Core Functionality
- Bug fixes and improvements for Editor UI.

## n8n@0.139.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.138.0...n8n@0.139.0) for this version.<br />
**Release date:** 2021-09-22

### New nodes

* [Elastic Security](/integrations/builtin/app-nodes/n8n-nodes-base.elasticsecurity/)
* [Misp](/integrations/builtin/app-nodes/n8n-nodes-base.misp/)
* [Netlify](/integrations/builtin/app-nodes/n8n-nodes-base.netlify/)
* [Netlify Trigger](/integrations/builtin/trigger-nodes/n8n-nodes-base.netlifytrigger/)

### Enhanced nodes

* [HubSpot Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.hubspottrigger/) Authentication method changed to OAuth2.
* [Wait:](/integrations/builtin/core-nodes/n8n-nodes-base.wait/) Added improved status messages for Wait behavior.

### Core Functionality
- Updated node design to include support for versioned nodes.

### Bug fixes

* [SendGrid:](/integrations/builtin/app-nodes/n8n-nodes-base.sendgrid/) Fixed issue with adding contacts to lists.

### Contributors

[Matías Aguirre](https://github.com/omab)

## n8n@0.138.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.137.0...n8n@0.138.0) for this version.<br />
**Release date:** 2021-09-15

### New nodes

* [Item Lists](/integrations/builtin/core-nodes/n8n-nodes-base.itemlists/)
* [Magento 2](/integrations/builtin/app-nodes/n8n-nodes-base.magento2/)

### Enhanced nodes

* [Baserow:](/integrations/builtin/app-nodes/n8n-nodes-base.baserow/) Added the following filter options: Contains, Contains Not, Date Before Date, Date After Date, Filename Contains, Is Empty, Is Not Empty, Link Row Has, Link Row Does Not Have, Single Select Equal, and Single Select Not Equal.
* [Pipedrive:](/integrations/builtin/app-nodes/n8n-nodes-base.pipedrive/) Added support for Notes on Leads.
* [WeKan:](/integrations/builtin/app-nodes/n8n-nodes-base.wekan/) Added Sort field to the Card resource.


### Core Functionality

- General UX improvements to the Editor UI.
- Fixed an issue with the `PayloadTooLargeError`.

### Bug fixes

* [Lemlist:](/integrations/builtin/app-nodes/n8n-nodes-base.lemlist/) Fixed issue where events were not sent in the correct property.
* [Notion:](/integrations/builtin/app-nodes/n8n-nodes-base.notion/) Fixed issue listed unnamed databases.

### Contributors

[bramknuever](https://github.com/bramknuever), [Chris Magnuson](https://github.com/ChrisMagnuson)

## n8n@0.137.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.136.0...n8n@0.137.0) for this version.<br />
**Release date:** 2021-09-05

### New nodes

* [Freshservice](/integrations/builtin/app-nodes/n8n-nodes-base.freshservice/)

### Enhanced nodes

* [Clockify:](/integrations/builtin/app-nodes/n8n-nodes-base.clockify/) Added Task resource.
* [HubSpot:](/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/) Added dropdown selection for Properties and Properties with History filters for Get All Deals operations.
* [Mautic:](/integrations/builtin/app-nodes/n8n-nodes-base.mautic/) Added Campaign Contact resource.
* [MongoDB:](/integrations/builtin/app-nodes/n8n-nodes-base.mongodb/) Added ability to query documents by '_id'.
* [MQTT:](/integrations/builtin/app-nodes/n8n-nodes-base.mqtt/) Added SSL/TLS support to authentication.
* [MQTT Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.mqtttrigger/) Added SSL/TLS support to authentication.
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Added File Extension option to the Document resource. Added Type field to Task resource.
* [Sms77:](/integrations/builtin/app-nodes/n8n-nodes-base.sms77/) Added Voice Call resource. Added the following options to SMS resource: Debug, Delay, Foreign ID, Flash, Label, No Reload, Performance Tracking, TTL.
* [Zendesk:](/integrations/builtin/app-nodes/n8n-nodes-base.zendesk/) Added Organization resource. Added Get Organizations and Get Related Data operations to User resource.

### Core Functionality

- Added execution ID to logs of queue processes.
- Added description to operation errors.
- Added ability for webhook processes to wake waiting executions.

### Bug fixes

* [HubSpot:](/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/) Fixed issue with 'RequestAllItems' API.
* [WordPress:](/integrations/builtin/app-nodes/n8n-nodes-base.wordpress/) Fixed issue with 'RequestAllItems' API only returning the first 10 items.

### Contributors

[André Matthies](https://github.com/matthiez), [DeskYT](https://github.com/DeskYT), [Frederic Alix](https://github.com/fredericalix), [Jonathan Bennetts](https://github.com/Joffcom), [Ketan Somvanshi](https://github.com/KetanSomvanshi), [Luiz Eduardo de Oliveira Fonseca](https://github.com/luizeof), [TheFSilver](https://github.com/TheFSilver)

## n8n@0.136.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.135.3...n8n@0.136.0) for this version.<br />
**Release date:** 2021-08-30

### Enhanced nodes

* [Notion:](/integrations/builtin/app-nodes/n8n-nodes-base.notion/) Added handling of Rich Text when simplifying data.

### Core Functionality
- General UI design improvements.
- Improved errors messages during debugging of custom nodes.
- All packages upgraded to TypeScript 4.3.5, improved linting and formatting.

### Bug fixes

* [FTP:](/integrations/builtin/core-nodes/n8n-nodes-base.ftp/) Fixed issue where incorrect paths were displayed when using the node.
* [Wait:](/integrations/builtin/core-nodes/n8n-nodes-base.wait/) Fixed issue when receiving multiple files using On Webhook Call operation.
* [Webhook:](/integrations/builtin/core-nodes/n8n-nodes-base.webhook/) Fixed issue when receiving multiple files.


## n8n@0.135.3
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.135.2...n8n@0.135.3) for this version.<br />
**Release date:** 2021-08-27

### Core Functionality
- Fixed Canvas UI inconsistencies when duplicating workflows.
- Added log message during upgrade to indicate database migration has started.
- General improvements to parameter labels and tooltips.

### Contributors

[Kyle Mohr](https://github.com/kylefmohr)


## n8n@0.135.2
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.135.1...n8n@0.135.2) for this version.<br />
**Release date:** 2021-08-26

### Core Functionality

- Added expression support for credentials.
- Fixed performance issues when loading credentials.

## n8n@0.135.1

For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.135.0...n8n@0.135.1) for this version.<br />
**Release date:** 2021-08-23

### Core Functionality
- Fixed an issue where if n8n was shutdown during database migration while upgrading versions, errors would result upon next startup.

## n8n@0.135.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.134.0...n8n@0.135.0) for this version.<br />
**Release date:** 2021-08-22

/// warning | Breaking changes
Please note that this version contains breaking changes. You can read more about it [here](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01350).
The features that introduced the breaking changes have been flagged below.
///


### New nodes

* [Form.io Trigger](/integrations/builtin/trigger-nodes/n8n-nodes-base.formiotrigger/)
* [Formstack Trigger](/integrations/builtin/trigger-nodes/n8n-nodes-base.formstacktrigger/)
* [Wait](/integrations/builtin/core-nodes/n8n-nodes-base.wait/)

### Core Functionality
- In-node method for accessing binary data is now asynchronous and a helper function for this has been implemented. [](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01350)
- Credentials are now loaded from the database on-demand. [](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01350)
- Webhook UUIDs are automatically updated when duplicating a workflow.
- Fixed an issue when referencing values before loops.

### Bug fixes

* [Interval:](/integrations/builtin/core-nodes/n8n-nodes-base.interval/) Fixed issue where entering too large a value (> 2147483647ms) resulted in an interval of 1sec being used rather than an error.

### Contributors

[Aniruddha Adhikary](https://github.com/aniruddha-adhikary), [lublak](https://github.com/lublak), [parthibanbalaji](https://github.com/parthibanbalaji)


## n8n@0.134.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.133.0...n8n@0.134.0) for this version.<br />
**Release date:** 2021-08-15

### Enhanced nodes

* [AWS DynamoDB:](/integrations/builtin/app-nodes/n8n-nodes-base.awsdynamodb/) Added Scan option to Item > Get All operation.
* [Google Drive:](/integrations/builtin/app-nodes/n8n-nodes-base.googledrive/) Added File Name option to File > Update operation.
* [Mautic:](/integrations/builtin/app-nodes/n8n-nodes-base.mautic/) Added the following fields to Company resource: Address, Annual Revenue, Company Email, Custom Fields, Description, Fax, Industry, Number of Employees, Phone, Website.
* [Notion:](/integrations/builtin/app-nodes/n8n-nodes-base.notion/) Added Timezone option when inserting Date fields.
* [Pipedrive:](/integrations/builtin/app-nodes/n8n-nodes-base.pipedrive/) Added the following Filters options to the Deal > Get All operation: Predefined Filter, Stage ID, Status, and User ID.
* [QuickBooks:](/integrations/builtin/app-nodes/n8n-nodes-base.quickbooks/) Added the Transaction resource and Get Report operation.

### Core Functionality
- Integrated [Nodelinter](/integrations/creating-nodes/test/node-linter/) in n8n.
- Fix to add a trailing slash (`/`) to all webhook URLs for proper functionality.

### Bug fixes

* [AWS SES:](/integrations/builtin/app-nodes/n8n-nodes-base.awsses/) Fixed issue where special characters in the message were not encoded.
* [Baserow:](/integrations/builtin/app-nodes/n8n-nodes-base.baserow/) Fixed issue where Create operation inserted null values.
* [HubSpot:](/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/) Fixed issue when sending context parameter.

### Contributors

[calvintwr](https://github.com/calvintwr), [CFarcy](https://github.com/CFarcy), [Jeremie Dokime](https://github.com/dokime7), [Michael Hirschler](https://github.com/mvhirsch), [Rodrigo Correia](https://github.com/rodrigoscdc), [sol](https://github.com/5pecia1)

## n8n@0.133.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n%400.132.2...n8n@0.133.0) for this version.<br />
**Release date:** 2021-08-08

### New nodes

* [Monica CRM](/integrations/builtin/app-nodes/n8n-nodes-base.monicacrm/)

### Enhanced nodes

* [HTTP Request:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Added Follow All Redirects option.
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Added Record Type ID field.

### Core Functionality
- Fixed UI lag when editing large workflows.

### Bug fixes

* [Nextcloud:](/integrations/builtin/app-nodes/n8n-nodes-base.nextcloud/) Fixed issue where List operation on an empty Folder returned an error.
* [Spotify:](/integrations/builtin/app-nodes/n8n-nodes-base.spotify/) Fixed issues with pagination and infinite executions.

### Contributors

[Jacob Burrell](https://github.com/jacobburrell), [Лебедев Иван](https://github.com/X-pech)

## n8n@0.132.2
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.132.1...n8n@0.132.2) for this version.<br />
**Release date:** 2021-08-02

### Bug fixes

* [Interval:](/integrations/builtin/core-nodes/n8n-nodes-base.interval/) Fixed issue with infinite executions.

### Contributors

[Лебедев Иван](https://github.com/X-pech)

## n8n@0.132.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.132.0...n8n@0.132.1) for this version.<br />
**Release date:** 2021-08-02

### Core Functionality
- Changed TypeORM version to 0.2.34

## n8n@0.132.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.131.0...n8n@0.132.0) for this version.<br />
**Release date:** 2021-08-01

### New nodes

* [Freshworks CRM](/integrations/builtin/app-nodes/n8n-nodes-base.freshworkscrm/)
* [Google Perspective](/integrations/builtin/app-nodes/n8n-nodes-base.googleperspective/)
* [Marketstack](/integrations/builtin/app-nodes/n8n-nodes-base.marketstack/)
* [NocoDB](/integrations/builtin/app-nodes/n8n-nodes-base.nocodb/)


### Enhanced nodes

* [Facebook Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.facebooktrigger/) Added Fields parameter.
* [Gmail:](/integrations/builtin/app-nodes/n8n-nodes-base.gmail/) Added Sender Name parameter.
* [Home Assistant:](/integrations/builtin/app-nodes/n8n-nodes-base.homeassistant/) Added Event resource.
* [Pipedrive:](/integrations/builtin/app-nodes/n8n-nodes-base.pipedrive/) Added Deal Product resource.
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Added Document resource with Upload operation.
* [WooCommerce:](/integrations/builtin/app-nodes/n8n-nodes-base.woocommerce/) Added Customer resource.


### Core Functionality
- Fixed an issue for large internal values.

### Contributors

[Ed Linklater](https://github.com/edlinklater), [Rodrigo Correia](https://github.com/rodrigoscdc)

## n8n@0.131.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.130.0...n8n@0.131.0) for this version.<br />
**Release date:** 2021-07-24

/// warning | Breaking change
Please note that this version contains a breaking change. You can read more about it [here](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01310).
The features that introduced the breaking changes have been flagged below.
///


### New nodes

* [Webex by Cisco](/integrations/builtin/app-nodes/n8n-nodes-base.ciscowebex/)
* [Webex by Cisco Trigger](/integrations/builtin/trigger-nodes/n8n-nodes-base.ciscowebextrigger/)


### Enhanced nodes

* [Pipedrive:](/integrations/builtin/app-nodes/n8n-nodes-base.pipedrive/) Added Lead resource. Added Search operation to Organization resource.
* [Taiga Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.taigatrigger/) Added Resource and Operations filters.


### Core Functionality
- Added Continue-on-fail support to all nodes.
- Added new version notifications.
- Added Refresh List for remote options lists.
- Added `$position` expression variable to return the index of an item within a list.

### Bug fixes

* [Spreadsheet File:](/integrations/builtin/core-nodes/n8n-nodes-base.spreadsheetfile/) Fixed issue when saving dates.

### Contributors

[Anthr@x](https://github.com/AnthraX1), [Felipe Cecagno](https://github.com/fcecagno)

## n8n@0.130.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.129.0...n8n@0.130.0) for this version.<br />
**Release date:** 2021-07-18

/// warning | Breaking change
Please note that this version contains a breaking change. You can read more about it [here](https://github.com/n8n-io/n8n/  blob/master/packages/cli/BREAKING-CHANGES.md#01300).
The features that introduced the breaking changes have been flagged below.
///



### New nodes

* [AWS DynamoDB](/integrations/builtin/app-nodes/n8n-nodes-base.awsdynamodb/)
* [Elasticsearch](/integrations/builtin/app-nodes/n8n-nodes-base.elasticsearch/)
* [ServiceNow](/integrations/builtin/app-nodes/n8n-nodes-base.servicenow/)

### Enhanced nodes

* [Kafka Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.kafkatrigger/) Added Read Messages From Beginning option.
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Added Sandbox Environment Type for OAuth2 credentials.
* [Taiga:](/integrations/builtin/app-nodes/n8n-nodes-base.taiga/) Added Epic, Task, and User Story operations.
* [TheHive:](/integrations/builtin/app-nodes/n8n-nodes-base.thehive/) Added Custom Fields option to the available Additional Fields.

### Core Functionality
- Fixed an issue where failed workflows were displayed as "running".
- Fixes issues with uncaught errors.

### Bug fixes

* [Notion:](/integrations/builtin/app-nodes/n8n-nodes-base.notion/) Fixed issue when filtering field data type.

### Contributors

[Michael Hirschler](https://github.com/mvhirsch), [Mika Luhta](https://github.com/mluhta), [Pierre Lanvin](https://github.com/planvin)

## n8n@0.129.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.128.0...n8n@0.129.0) for this version.<br />
**Release date:** 2021-07-12

### New nodes

* [Baserow](/integrations/builtin/app-nodes/n8n-nodes-base.baserow/)

### Bug fixes

* [SSH:](/integrations/builtin/core-nodes/n8n-nodes-base.ssh/) Fixed issue with access rights when downloading files.

### Contributors

[Jérémie Pardou-Piquemal](https://github.com/jrmi)

## n8n@0.128.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.127.0...n8n@0.128.0) for this version.<br />
**Release date:** 2021-07-11

### New nodes

* [Home Assistant](/integrations/builtin/app-nodes/n8n-nodes-base.homeassistant/)
* [Stripe](/integrations/builtin/app-nodes/n8n-nodes-base.stripe/)

### Enhanced nodes

* [HTTP Request:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Added support for arrays in Querystring. Any parameter appearing multiple times with the same name is grouped into an array.
* [Mautic:](/integrations/builtin/app-nodes/n8n-nodes-base.mautic/) Added Contact Segment resource.
* [Telegram:](/integrations/builtin/app-nodes/n8n-nodes-base.telegram/) Added Delete operation to the Message resource.

### Core Functionality
- Performance improvement for loading of historical executions (> 3mil) when using Postgres.
- Fixed error handling for unending workflows and display of "unknown" workflow status.
- Fixed format of Workflow ID when downloading from UI Editor to enable compatibility with importing from CLI.

### Bug fixes

* [Microsoft SQL:](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftsql/) Fixed an issue with sending the connectionTimeout parameter, and creating and updating data using columns with spaces.

### Contributors

[Kaito Udagawa](https://github.com/umireon), [Rodrigo Correia](https://github.com/rodrigoscdc)


## n8n@0.127.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.126.1...n8n@0.127.0) for this version.<br />
**Release date:** 2021-07-04

/// warning | Breaking change
Please note that this version contains a breaking change. You can read more about it [here](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01270).
The features that introduced the breaking changes have been flagged below.
///


### Enhanced nodes

* [Airtable:](/integrations/builtin/app-nodes/n8n-nodes-base.airtable/) Added Bulk Size option to all Operations.
* [Box:](/integrations/builtin/app-nodes/n8n-nodes-base.box/) Added Share operation to File and Folder resources.
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Added Last Name field to Update operation on Contact resource.
* [Zoho CRM:](/integrations/builtin/app-nodes/n8n-nodes-base.zohocrm/) Added Account, Contact, Deal, Invoice, Product, Purchase, Quote, Sales Order, and Vendor resources.

### Core Functionality
- Added a workflow testing framework using a new CLI command to execute all desired workflows. Run `n8n executeBatch --help` for details.
- Added support to display binary video content in Editor UI.

### Bug fixes

* [Google Sheets:](/integrations/builtin/app-nodes/n8n-nodes-base.googlesheets/) Fixed an issue with handling 0 value that resulted in empty cells.
* [SSH:](/integrations/builtin/core-nodes/n8n-nodes-base.ssh/) Fixed an issue with setting passphrases.

### Contributors

[flybluewolf](https://github.com/flybluewolf), [Kaito Udagawa](https://github.com/umireon)

## n8n@0.126.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.126.0...n8n@0.126.1) for this version.<br />
**Release date:** 2021-06-29

### Core Functionality
- Fixed issues with keyboard shortcuts when a modal was open.

### Bug fixes

* [Microsoft SQL:](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftsql/) Fixed an issue with handling of Boolean values when inserting.
* [Pipedrive:](/integrations/builtin/app-nodes/n8n-nodes-base.pipedrive/) Fixed an issue with the node icon.

## n8n@0.126.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.125.0...n8n@0.126.0) for this version.<br />
**Release date:** 2021-06-27

### New nodes

* [Action Network](/integrations/builtin/app-nodes/n8n-nodes-base.actionnetwork/)
* [Google Docs](/integrations/builtin/app-nodes/n8n-nodes-base.googledocs/)

### Enhanced nodes

* [AWS S3:](/integrations/builtin/app-nodes/n8n-nodes-base.awsS3/) Added Delete operation to the Bucket Resource.
* [Google Analytics:](/integrations/builtin/app-nodes/n8n-nodes-base.googleanalytics/) Added Dimension Filters to the available Additional Fields.
* [HTTP Request:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Added Split Into Items option.
* [MQTT:](/integrations/builtin/app-nodes/n8n-nodes-base.mqtt/) Added mqqts protocol for MQTT credentials.
* [QuickBooks:](/integrations/builtin/app-nodes/n8n-nodes-base.quickbooks/) Added Purchase resource with Get and Get All operations.


### Core Functionality
- Templates from the [n8n Workflows](https://n8n.io/workflows) page can now be directly imported by appending `/workflows/templates/<templateId>` to your instance base URL. For example, `localhost:5678/workflows/templates/1142`.
- Added new Editor UI shortcuts. See [Keyboard Shortcuts](/keyboard-shortcuts/) for details.
- Fixed an issue causing console errors when deleting a node from the canvas.

### Bug fixes

* [Ghost:](/integrations/builtin/app-nodes/n8n-nodes-base.ghost/) Fixed an issue with the Get All operation functionality.
* [Google Analytics:](/integrations/builtin/app-nodes/n8n-nodes-base.googleanalytics/) Fixed an issue that caused an error when attempting to sort with no data present.
* [Microsoft SQL:](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftsql/) Fixed an issue when escaping single quotes and mapping empty fields.
* [Notion:](/integrations/builtin/app-nodes/n8n-nodes-base.notion/) Fixed an issue with pagination of databases and users.

### Contributors

[calvintwr](https://github.com/calvintwr), [Jan Baykara](https://github.com/janbaykara)

## n8n@0.125.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.124.1...n8n@0.125.0) for this version.<br />
**Release date:** 2021-06-20

### Enhanced nodes

* [Spotify:](/integrations/builtin/app-nodes/n8n-nodes-base.spotify/) Added Search operation to Album, Artist, Playlist, and Track resources, and Resume and Volume operations to Player resource.

### Core Functionality
- Implemented new design of the Nodes Panel, adding categories and subcategories, along with improved search. For full details, see the [commits](https://github.com/n8n-io/n8n/commit/0470740737c5ee199447a68b7277c43be2042976).

### Bug fixes

* [MySQL:](/integrations/builtin/app-nodes/n8n-nodes-base.mysql/) Fixed an issue where n8n was unable to save data due to collation, resulting in workflows ending with Unknown status.

### Contributors

[Amudhan Manivasagam](https://github.com/smamudhan), [Carlos Alexandro Becker](https://github.com/caarlos0), [Kaito Udagawa](https://github.com/umireon)

## n8n@0.124.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.124.0...n8n@0.124.1) for this version.<br />
**Release date:** 2021-06-16

### Core Functionality
- Improved error log messages
- Fixed an issue where the tags got removed when deactivating the workflow or updating settings
- Removed the circular references for the error caused by the request library

## n8n@0.124.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.123.1...n8n@0.124.0) for this version.<br />
**Release date:** 2021-06-13

### Enhanced nodes

* [Google Drive:](/integrations/builtin/app-nodes/n8n-nodes-base.googledrive/) Added APP Properties and Properties options to the Upload operation of the File resource
* [HTTP Request:](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/) Added the functionality to log the request to the browser console for testing
* [Notion:](/integrations/builtin/app-nodes/n8n-nodes-base.notion/) Added the Include Time parameter date field types
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Added Upsert operation to Account, Contact, Custom Object, Lead, and Opportunity resources
* [Todoist:](/integrations/builtin/app-nodes/n8n-nodes-base.todoist/) Added the Description option to the Task resource

### Core Functionality
- Implemented the functionality to display the error details in a toast message for trigger nodes
- Improved error handling by removing circular references from API errors

### Bug fixes

* [Jira:](/integrations/builtin/app-nodes/n8n-nodes-base.jira/) Fixed an issues with the API version and fixed an issue with fetching the custom fields for the Issue resource

### Contributors


[Jean M](https://github.com/jemos), [romaincolombo-daily](https://github.com/romaincolombo-daily), [Thomas Jost](https://github.com/Schnouki), [Vincent](https://github.com/vbouchet31)

## n8n@0.123.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.123.0...n8n@0.123.1) for this version.<br />
**Release date:** 2021-06-06

### Core Functionality
- Fixed a build issue for missing node icons

## n8n@0.123.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.122.3...n8n@0.123.0) for this version.<br />
**Release date:** 2021-06-06

### New nodes

* [Git](/integrations/builtin/core-nodes/n8n-nodes-base.git/)
* [Microsoft To Do](/integrations/builtin/app-nodes/n8n-nodes-base.microsofttodo/)

### Enhanced nodes

* [Pipedrive:](/integrations/builtin/app-nodes/n8n-nodes-base.pipedrive/) Added a feature to fetch data from the Pipedrive API, added Search operation to the Deals resource, and added custom fields option
* [Spotify:](/integrations/builtin/app-nodes/n8n-nodes-base.spotify/) Added My Data resource

### Core Functionality
- Fixed issues with NodeViewNew navigation handling
- Fixed an issue with the view crashing with large requests

### Bug fixes

* [ASW Transcribe:](/integrations/builtin/app-nodes/n8n-nodes-base.awstranscribe/) Fixed issues with options

### Contributors


[Rodrigo Correia](https://github.com/rodrigoscdc), [Sam Roquitte](https://github.com/samr28)

## n8n@0.122.3
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.122.2...n8n@0.122.3) for this version.<br />
**Release date:** 2021-06-04

### Core Functionality
- Fixed error messages for the text area field
- Added the missing `winston` dependency
- Fixed an issue with adding values using the Variable selector. The deleted values don't reappear
- Fixed an issue with the Error Workflows not getting executed in the queue mode

### Bug fixes

* [Notion:](/integrations/builtin/app-nodes/n8n-nodes-base.notion/) Fixed an issue with parsing the last edited time

## n8n@0.122.2
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.122.1...n8n@0.122.2) for this version.<br />
**Release date:** 2021-05-31

### Enhanced nodes

* [Function:](/integrations/builtin/core-nodes/n8n-nodes-base.function/) Added console.log support for writing to browser console
* [Function Item:](/integrations/builtin/core-nodes/n8n-nodes-base.functionitem/) Added console.log support for writing to browser console

### Core Functionality
- Fixed an issue that enables clicks on tags
- Fixed an issue with escaping workflow name
- Fixed an issue with selecting variables in the Expression Editor

## n8n@0.122.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.122.0...n8n@0.122.1) for this version.<br />
**Release date:** 2021-05-30

### Core Functionality
- Fixed an issue with the order in migration rollback

## n8n@0.122.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.121.0...n8n@0.122.0) for this version.<br />
**Release date:** 2021-05-30

### New nodes

* [AWS Transcribe](/integrations/builtin/app-nodes/n8n-nodes-base.awstranscribe/)
* [SSH](/integrations/builtin/core-nodes/n8n-nodes-base.ssh/)
* [UptimeRobot](/integrations/builtin/app-nodes/n8n-nodes-base.uptimerobot/)

### Enhanced nodes

* [DeepL:](/integrations/builtin/app-nodes/n8n-nodes-base.deepl/) Added support for Free API
* [Function:](/integrations/builtin/core-nodes/n8n-nodes-base.function/) Added the functionality to log console.log messages to the browser console
* [Function Item:](/integrations/builtin/core-nodes/n8n-nodes-base.functionitem/) Added the functionality to log console.log messages to the browser console

### Core Functionality
- Changed `bcrypt` library from `@node-rs/bcrypt` to `bcryptjs`
- Fixed an issue with optional parameters that have the same name
- Added the functionality to tag workflows
- Fixed errors in the Expression Editor
- Fixed an issue with nodes that only get connected to the second input. This solves the issue of copying and pasting the workflows where only one output of the IF node gets connected to a node

### Bug fixes

* [Google Drive:](/integrations/builtin/app-nodes/n8n-nodes-base.googledrive/) Fixed an issue with the Drive resource
* [Notion:](/integrations/builtin/app-nodes/n8n-nodes-base.notion/) Fixed an issue with the filtering fields type and fixed an issue with the link option
* [Switch:](/integrations/builtin/core-nodes/n8n-nodes-base.switch/) Fixed an issue with the Expression mode

### Contributors


[Alexander Mustafin](https://github.com/sashker)

## n8n@0.121.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.121.0...n8n@0.121.1) for this version.<br />
**Release date:** 2021-06-01

### Core Functionality
- Fixed an issue with copying the output values
- Fixed issues with the Expression Editor
- Made improvements to the Expression Editor

## n8n@0.121.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.120.0...n8n@0.121.0) for this version.<br />
**Release date:** 2021-05-20

### New nodes

* [Notion](/integrations/builtin/app-nodes/n8n-nodes-base.notion/)
* [Notion Trigger](/integrations/builtin/trigger-nodes/n8n-nodes-base.notiontrigger/)

### Enhanced nodes

* [GraphQL:](/integrations/builtin/core-nodes/n8n-nodes-base.graphql/) Added Header Auth authentication method
* [Twilio:](/integrations/builtin/app-nodes/n8n-nodes-base.twilio/) Added API Key authentication method

### Bug fixes

* [HubSpot:](/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/) Fixed an issue with pagination for Deals resource
* [Keap:](/integrations/builtin/app-nodes/n8n-nodes-base.keap/) Fixed an issue with the data type of the Order Title field
* [Orbit:](/integrations/builtin/app-nodes/n8n-nodes-base.orbit/) Fixed an issue with the activity type in Post operation
* [Slack:](/integrations/builtin/app-nodes/n8n-nodes-base.slack/) Fixed an issue with the Get Profile operation
* [Strava:](/integrations/builtin/app-nodes/n8n-nodes-base.strava/) Fixed an issue with the paging parameter

### Contributors


[Jacob Spizziri](https://github.com/jspizziri)

## n8n@0.120.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.119.0...n8n@0.120.0) for this version.<br />
**Release date:** 2021-05-17

### New nodes

* [iCalendar](/integrations/builtin/core-nodes/n8n-nodes-base.ical/)

### Enhanced nodes

* [Google Cloud Firestore:](/integrations/builtin/app-nodes/n8n-nodes-base.googlecloudfirestore/) Added the functionality for GeoPoint parsing and added ISO-8601 format for date validation
* [IMAP Email:](/integrations/builtin/core-nodes/n8n-nodes-base.emailimap/) Added the Force reconnect option
* [Paddle:](/integrations/builtin/app-nodes/n8n-nodes-base.paddle/) Added the Use Sandbox environment API parameter
* [Spotify:](/integrations/builtin/app-nodes/n8n-nodes-base.spotify/) Added the Position parameter to the Add operation of the Playlist resource
* [WooCommerce:](/integrations/builtin/app-nodes/n8n-nodes-base.woocommerce/) Added the Include Credentials in Query parameter

### Core Functionality
- Added await to hooks to fix issues with the `Unknown` status of the workflows
- Changed the data type of the `credentials_entity` field for MySQL database to fix issues with long credentials
- Fixed an issue with the ordering of the executions when the list is auto-refreshed
- Added the functionality that allows reading sibling parameters

### Bug fixes

* [Clockify Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.clockifytrigger/) Fixed an issue that occurred when the node returned an empty array
* [Google Cloud Firestore:](/integrations/builtin/app-nodes/n8n-nodes-base.googlecloudfirestore/) Fixed an issue with parsing empty document, and an issue with the detection of date
* [HubSpot:](/integrations/builtin/app-nodes/n8n-nodes-base.hubspot/) Fixed an issue with the Return All option

### Contributors


[DeskYT](https://github.com/DeskYT), [Daniel Lazaro](https://github.com/1izardo), [DerEnderKeks](https://github.com/DerEnderKeks), [mdasmendel](https://github.com/mdasmendel)

## n8n@0.119.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.118.1...n8n@0.119.0) for this version.<br />
**Release date:** 2021-05-09

### Enhanced nodes

* [AWS Comprehend:](/integrations/builtin/app-nodes/n8n-nodes-base.awscomprehend/) Added the Detect Entities operation
* [AWS Lambda:](/integrations/builtin/app-nodes/n8n-nodes-base.awslambda/) Added the ability to list functions recursively if the number of functions exceeds 50
* [Google Analytics:](/integrations/builtin/app-nodes/n8n-nodes-base.googleanalytics/) Added pagination to the Report resource
* [Mailjet:](/integrations/builtin/app-nodes/n8n-nodes-base.mailjet/) Added Reply To parameter
* [Redis:](/integrations/builtin/app-nodes/n8n-nodes-base.redis/) Added the Increment operation
* [Spreadsheet File:](/integrations/builtin/core-nodes/n8n-nodes-base.spreadsheetfile/) Added the Header Row option
* [Webflow Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.webflowtrigger/) Added Collection Item Created, Collection Item Updated, and Collection Item Deleted events

### Core Functionality
- Implemented timeout for subworkflows
- Removed the deregistration webhooks functionality from the webhook process

### Bug fixes

* [Google Cloud Firestore:](/integrations/builtin/app-nodes/n8n-nodes-base.googlecloudfirestore/) Fixed an issue with parsing null value
* [Google Sheets:](/integrations/builtin/app-nodes/n8n-nodes-base.googlesheets/) Fixed an issue with the Key Row parameter
* [HubSpot:](/integrations/builtin/app-nodes/n8n-nodes-base.zohocrm/) Fixed an issue with the authentication

### Contributors


[Nikita](https://github.com/Rirush)


## n8n@0.118.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.118.0...n8n@0.118.1) for this version.<br />
**Release date:** 2021-05-05

### Core Functionality

- Fixed an issue with error workflows

## n8n@0.118.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.117.0...n8n@0.118.0) for this version.<br />
**Release date:** 2021-05-02

/// warning | Breaking change
Please note that this version contains a breaking change. You can read more about it [here](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01180).
The features that introduced the breaking changes have been flagged below.
///

### New nodes

* [Kitemaker](/integrations/builtin/app-nodes/n8n-nodes-base.kitemaker/)
* [MQTT](/integrations/builtin/app-nodes/n8n-nodes-base.mqtt/)

### Enhanced nodes

* [CrateDB:](/integrations/builtin/app-nodes/n8n-nodes-base.cratedb/) Added query parameters. The Execute Query operation returns the result from all queries executed instead of just one of the results.
* [ERPNext:](/integrations/builtin/app-nodes/n8n-nodes-base.erpnext/) Added support for self-hosted ERPNext instances
* [FTP:](/integrations/builtin/core-nodes/n8n-nodes-base.ftp/) Added the functionality to delete folders
* [Google Calendar:](/integrations/builtin/app-nodes/n8n-nodes-base.googlecalendar/) Added the Continue on Fail functionality
* [Google Drive:](/integrations/builtin/app-nodes/n8n-nodes-base.googledrive/) Added the functionality to add file name when downloading files
* [Gmail:](/integrations/builtin/app-nodes/n8n-nodes-base.gmail/) Added functionality to handle multiple binary properties
* [Microsoft Outlook:](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftoutlook/) Added Is Read and Move option to the Message resource
* [Postgres:](/integrations/builtin/app-nodes/n8n-nodes-base.postgres/) Added query parameters. The Execute Query operation returns the result from all queries executed instead of just one of the results.
* [QuestDB:](/integrations/builtin/app-nodes/n8n-nodes-base.questdb/) Added query parameters. The Execute Query operation returns the result from all queries executed instead of just one of the results.
* [QuickBase:](/integrations/builtin/app-nodes/n8n-nodes-base.quickbase/) Added option to use Field IDs
* [TimescaleDB:](/integrations/builtin/app-nodes/n8n-nodes-base.timescaledb/) Added query parameters. The Execute Query operation returns the result from all queries executed instead of just one of the results.
* [Twist:](/integrations/builtin/app-nodes/n8n-nodes-base.twist/) Added Get, Get All, Delete, and Update operations to the Message Conversation resource. Added Archive, Unarchive, and Delete operations to the Channel resource. Added Thread and Comment resource

### Core Functionality
- Implemented the native `fs/promise` library where possible
- Added the functionality to output logs to the console or a file
- We have updated the minimum required version for Node.js to v14.15. For more details, check out the entry in the [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01180) page

### Bug fixes

* [GetResponse Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.getresponsetrigger/) Fixed an issue with error handling
* [GitHub Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.githubtrigger/) Fixed an issue with error handling
* [GitLab Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.gitlabtrigger/) Fixed an issue with error handling
* [Google Sheets:](/integrations/builtin/app-nodes/n8n-nodes-base.googlesheets/) Fixed an issue with the Lookup operation for returning empty rows
* [Orbit:](/integrations/builtin/app-nodes/n8n-nodes-base.orbit/) Fixed issues with the Post resource
* [Redis:](/integrations/builtin/app-nodes/n8n-nodes-base.redis/) Fixed an issue with the node not returning an error
* [Xero:](/integrations/builtin/app-nodes/n8n-nodes-base.xero/) Fixed an issue with the Create operation for the Contact resource

### Contributors


[Gustavo Arjones](https://github.com/arjones), [lublak](https://github.com/lublak), [Colton Anglin](https://github.com/Colton), [Mika Luhta](https://github.com/mluhta)


## n8n@0.117.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.116.1...n8n@0.117.0) for this version.<br />
**Release date:** 2021-04-24

/// warning | Breaking change
Please note that this version contains a breaking change. You can read more about it [here](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01170).
The features that introduced the breaking changes have been flagged below.
///


### New nodes

* [Mailcheck](/integrations/builtin/app-nodes/n8n-nodes-base.mailcheck/)
* [n8n Trigger](/integrations/builtin/core-nodes/n8n-nodes-base.n8nTrigger/)
* [Workflow Trigger](/integrations/builtin/core-nodes/n8n-nodes-base.workflowtrigger/)

### Enhanced nodes

* [CrateDB:](/integrations/builtin/app-nodes/n8n-nodes-base.cratedb/) Added the Mode option that allows you to execute queries as transactions
* [Nextcloud:](/integrations/builtin/app-nodes/n8n-nodes-base.nextcloud/) Added Delete, Get, Get All, and Update operation to the User resource
* [Postgres:](/integrations/builtin/app-nodes/n8n-nodes-base.postgres/) Added the Mode option that allows you to execute queries as transactions
* [QuestDB:](/integrations/builtin/app-nodes/n8n-nodes-base.questdb/) Added the Mode option that allows you to execute queries as transactions
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Added Owner option to the Case and Lead resources. Added custom fields to Create and Update operations of the Case resource
* [Sentry.io:](/integrations/builtin/app-nodes/n8n-nodes-base.sentryio/) Added Delete and Update operations to Project, Release, and Team resources
* [TimescaleDB:](/integrations/builtin/app-nodes/n8n-nodes-base.timescaledb/) Added the Mode option that allows you to execute queries as transactions
* [Zendesk Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.zendesktrigger/) Added support to retrieve custom fields

### Core Functionality
- The Activation Trigger node has been deprecated. It has been replaced by two new nodes - the n8n Trigger and the Workflow Trigger node. For more details, check out the entry in the [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01170) page
- Added the functionality to open the New Credentials dropdown by default

### Bug fixes

* [Google Sheets:](/integrations/builtin/app-nodes/n8n-nodes-base.googlesheets/) Fixed an issue with the Lookup operation for returning multiple empty rows
* [Intercom:](/integrations/builtin/app-nodes/n8n-nodes-base.intercom/) Fixed an issue with the User operation in the Company resource
* [Mautic:](/integrations/builtin/app-nodes/n8n-nodes-base.mautic/) Fixed an issue with sending the lastActive parameter

### Contributors


[Bart Vollebregt](https://github.com/bartvollebregt), [Ivan Timoshenko](https://github.com/bugagashenkj), [Konstantin Nosov](https://github.com/nosovk), [lublak](https://github.com/lublak), [Umair Kamran](https://github.com/UmairKamran),

## n8n@0.116.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.116.0...n8n@0.116.1) for this version.<br />
**Release date:** 2021-04-20

### Core Functionality
- Fixed a timeout issue with the workflows in the main process

## n8n@0.116.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.115.0...n8n@0.116.0) for this version.<br />
**Release date:** 2021-04-17

### New nodes

* [Google BigQuery](/integrations/builtin/app-nodes/n8n-nodes-base.googlebigquery/)
* [Webflow](/integrations/builtin/app-nodes/n8n-nodes-base.webflow/)

### Enhanced nodes

* [Date & Time:](/integrations/builtin/core-nodes/n8n-nodes-base.datetime/) Added Calculate a Date action that allows you to add or subtract time from a date
* [GitLab:](/integrations/builtin/app-nodes/n8n-nodes-base.gitlab/) Added Get, Get All, Update, and Delete operations to the Release resource
* [Microsoft OneDrive:](/integrations/builtin/app-nodes/n8n-nodes-base.microsoftonedrive/) Added Delete operation to the Folder resource
* [Monday:](/integrations/builtin/app-nodes/n8n-nodes-base.mondaycom/) Added support for OAuth2 authentication
* [MongoDB:](/integrations/builtin/app-nodes/n8n-nodes-base.mongodb/) Added Limit, Skip, and Sort options to the Find operation and added Upsert parameter to the Update operation. Added the functionality to close the connection after use
* [MySQL:](/integrations/builtin/app-nodes/n8n-nodes-base.mysql/) Added support for insert modifiers and added support for SSL
* [RabbitMQ:](/integrations/builtin/app-nodes/n8n-nodes-base.rabbitmq/) Added the functionality to close the connection after use and added support for AMPQS

### Core Functionality

- Changed `bcrypt` library from `bcryptjs` to `@node-rs/bcrypt`
- Improved node error handling. Status codes and error messages in API responses have been standardized
- Added global timeout setting for all HTTP requests (except HTTP Request node)
- Implemented timeout for workers and corrected timeout for sub workflows

### Bug fixes

* [AWS SQS:](/integrations/builtin/app-nodes/n8n-nodes-base.awssqs/) Fixed an issue with API version and casing
* [IMAP:](/integrations/builtin/core-nodes/n8n-nodes-base.emailimap/) Fixed re-connection issue
* [Keap:](/integrations/builtin/app-nodes/n8n-nodes-base.keap/) Fixed an issue with the Opt In Reason parameter
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Fixed an issue with loading custom fields

### Contributors


[Allan Daemon](https://github.com/AllanDaemon), [Anton Romanov](https://github.com/theone74), [Bart Vollebregt](https://github.com/bartvollebregt), [Cassiano Vailati](https://github.com/cassvail), [entrailz](https://github.com/entrailz), [Konstantin Nosov](https://github.com/nosovk), [LongYinan](https://github.com/Brooooooklyn)

## n8n@0.115.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.114.0...n8n@0.115.0) for this version.<br />
**Release date:** 2021-04-10

### New nodes

* [Google Slides](/integrations/builtin/app-nodes/n8n-nodes-base.googleslides/)

### Enhanced nodes

* [GitHub:](/integrations/builtin/app-nodes/n8n-nodes-base.github/) Added Release resource
* [TheHive:](/integrations/builtin/app-nodes/n8n-nodes-base.thehive/) Added support to fetch observable data types
* [RabbitMQ:](/integrations/builtin/app-nodes/n8n-nodes-base.rabbitmq/) Added header parameters

### Core Functionality

- Fixed an issue with expressions not being displayed in read-only mode
- Fixed an issue that didn't allow editing JavaScript code in read-only mode
- Added support for configuring the maximum payload size
- Added support to dynamically add menu items

### Bug fixes

* [Jira:](/integrations/builtin/app-nodes/n8n-nodes-base.jira/) Fixed an issue with loading issue types with classic project type
* [RabbitMQ Trigger:](/integrations/builtin/trigger-nodes/n8n-nodes-base.rabbitmqtrigger/) Fixed an issue with the node reusing the same item
* [SendGrid:](/integrations/builtin/app-nodes/n8n-nodes-base.sendgrid/) Fixed an issue with the dynamic field generation

### Contributors


[Mika Luhta](https://github.com/mluhta), [Loran](https://github.com/loranmutafov), [stwonary](https://github.com/stwonary)

## n8n@0.114.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.113.0...n8n@0.114.0) for this version.<br />
**Release date:** 2021-04-03

### New nodes

* [AWS SQS](/integrations/builtin/app-nodes/n8n-nodes-base.awssqs/)
* [Copper](/integrations/builtin/app-nodes/n8n-nodes-base.copper/)
* [ERPNext](/integrations/builtin/app-nodes/n8n-nodes-base.erpnext/)
* [Oura](/integrations/builtin/app-nodes/n8n-nodes-base.oura/)

### Enhanced nodes

* [Google Drive:](/integrations/builtin/app-nodes/n8n-nodes-base.googledrive/) Added support for creating folders for shared drives
* [Google Sheets:](/integrations/builtin/app-nodes/n8n-nodes-base.googlesheets/) Added Create and Remove operation to the Sheet resource
* [Harvest:](/integrations/builtin/app-nodes/n8n-nodes-base.harvest/) Added Update operation to the Task resource
* [Jira:](/integrations/builtin/app-nodes/n8n-nodes-base.jira/) Added Reporter field to the Issue resource
* [Postgres:](/integrations/builtin/app-nodes/n8n-nodes-base.postgres/) Added support for type casting

### Core Functionality

- Fixed an issue with the Redis connection to prevent memory leaks

### Bug fixes

* [Bitwarden:](/integrations/builtin/app-nodes/n8n-nodes-base.bitwarden/) Fixed an issue with the Update operation of the Group resource
* [Cortex:](/integrations/builtin/app-nodes/n8n-nodes-base.cortex/) Fixed an issue where only the last item got returned
* [Invoice Ninja:](/integrations/builtin/app-nodes/n8n-nodes-base.invoiceninja/) Fixed an issue with the Project parameter
* [Salesforce:](/integrations/builtin/app-nodes/n8n-nodes-base.salesforce/) Fixed an issue with the Get All operation of the Custom Object resource

### Contributors


[Agata M](https://github.com/curryy), [Allan Daemon](https://github.com/AllanDaemon), [Craig McElroy](https://github.com/camcelroy), [mjysci](https://github.com/mjysci)

## n8n@0.113.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.112.0...n8n@0.113.0) for this version.<br />
**Release date:** 2021-03-26

- New nodes
- Activation Trigger
- Plivo
- Enhanced nodes
- ClickUp: Added Space Tag, Task List, and Task Tag resource
- GitHub: Added pagination to Get Issues and Get Repositories operations
- Mattermost: Added Reaction resource and Post Ephemeral operation
- Move Binary Data: Added Encoding and Add BOM option to JSON to Binary mode and Strip BOM to Binary to JSON mode
- SendGrid: Added Mail resource
- Spotify: Added Library resource
- Telegram: Added Answer Inline Query operation to the Callback resource
- uProc: Added Get ASIN code by EAN code, Get EAN code by ASIN code, Get Email by Social Profile, Get Email by Full name and Company's domain, and Get Email by Full name and Company's name operations
- Bug fixes
- Clearbit: Fixed an issue with the autocomplete URI
- Dropbox: Fixed an issue with the Dropbox credentials by adding the APP Access Type parameter in the credentials. For more details, check out the entry in the [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01130) page
- Spotify: Fixed an issue with the Delete operation of the Playlist resource
- The variable selector now displays empty arrays
- Fixed a permission issue with the Raspberry Pi Docker image

## n8n@0.112.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.111.0...n8n@0.112.0) for this version.<br />
**Release date:** 2021-03-19

- New nodes
- DeepL
- Enhanced nodes
- TheHive: Added Mark as Read and Mark as Unread operations and added Ignore SSL Issues parameter to the credentials
- Bug fixes
- AWS SES: Fixed an issue to map CC addresses correctly
- Salesforce: Fixed an issue with custom object for Get All operations and fixed an issue with the first name field for the Create and Update operations for the Lead resource
- Strava: Fixed an issue with the access tokens not getting refreshed
- TheHive: Fixed an issue with the case resolution status
- Fixed an issue with importing separate decrypted credentials
- Fixed issues with the sub-workflows not finishing
- Fixed an issue with the sub-workflows running on the main process
- Fixed concurrency issues with sub-workflows

## n8n@0.111.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.110.3...n8n@0.111.0) for this version.<br />
**Release date:** 2021-03-12

- New nodes
- Autopilot
- Autopilot Trigger
- Wise
- Wise Trigger
- Enhanced nodes
- Box: Added Get operation to the Folder resource
- Dropbox: Added Search operation to the File resource. All operations are now performed relative to the user's root directory. For more details, check out the entry in the [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01110) page
- Facebook Graph API: Added new API versions
- Google Drive: Added Update operation to the File resource
- HubSpot: Added the Deal Description option
- Kafka: Added the SASL mechanism
- Monday.com: Added Move operation to Board Item resource
- MongoDB: Added Date field to the Insert and Update operations
- Micrsoft SQL: Added connection timeout parameter to credentials
- Salesforce: Added Mobile Phone field to the Lead resource
- Spotify: Added Create a Playlist operation to Playlist resource and Get New Releases to the Album resource
- Bug fixes
- Airtable: Fixed a bug with updating and deleting records
- Added the functionality to expose metrics to Prometheus. Read more about that [here](/hosting/configuration/#prometheus)
- Updated fallback values to match the value type
- Added the functionality to display debugging information for pending workflows on exit
- Fixed an issue with queue mode for the executions that shouldn't be saved
- Fixed an issue with workflows crashing and displaying `Unknown` status in the execution list
- Fixed an issue to prevent crashing while saving execution data when the `data` field has over 64KB in MySQL
- Updated `jws-rsa` to version `1.12.1`

## n8n@0.110.3
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.110.0...n8n@0.110.3) for this version.<br />
**Release date:** 2021-03-04

- Bug fixes
- APITemplate.io: Fixed an issue with the naming of the node

## n8n@0.110.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.109.0...n8n@0.110.0) for this version.<br />
**Release date:** 2021-03-04

- New nodes
- APITemplate.io
- Bubble
- Lemlist
- Lemlist Trigger
- Enhanced nodes
- Microsoft Teams: Added option to reply to a message
- Bug fixes
- Dropbox: Fixed an issue with parsing the response with the Upload operation
- Gmail: Fixed an issue with the scope for the Service Account authentication method and fixed an issue with the label filter
- Google Drive: Fixed an issue with the missing Parent ID field for the Create operation and fixed an issue with the Permissions field
- HelpScout: Fixed an issue with sending tags when creating a conversation
- HTTP Request: Fixed an issue with the raw data and file response
- HubSpot: Fixed an issue with the OAuth2 credentials
- Added support for Date & Time in the IF node and the Switch node
- Fixed an issue with mouse selection when zooming in or out
- Fixed an issue with current executing workflows when using queues for Postgres
- Fixed naming and description for the `N8N_SKIP_WEBHOOK_DEREGISTRATION_SHUTDOWN` environment variable
- Fixed an issue with auto-refresh of the execution list

## n8n@0.109.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.108.0...n8n@0.109.0) for this version.<br />
**Release date:** 2021-02-22

- New nodes
- Bitwarden
- Emelia
- Emelia Trigger
- GoToWebinar
- Raindrop
- Enhanced nodes
- AWS Rekognition: Added the Detect Text type to the Analyze operation for the Image resource
- Google Calendar: Added RRULE parameter to the Get All operation for the Event resource
- Jira: Added User resource and operations
- Reddit: Added the Search operation for the Post resource
- Telegram: Added the Send Location operation
- Bug fixes
- RocketChat: Fixed error responses
- Fixed the issue which caused the execution history of subworkflows (workflows started using the Execute Workflow node) not to be saved
- Added an option to export the credential data in plain text format using the CLI

## n8n@0.108.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.107.0...n8n@0.108.0) for this version.<br />
**Release date:** 2021-02-15

- New nodes
- Demio
- PostHog
- QuickBooks
- Enhanced nodes
- Trello: Added Create Checklist Item operation to the Checklist resource
- Webhook: Removed trailing slash in routes and updated logic to select dynamic webhook
- Bug fixes
- Google Drive: Fixed an issue with returning the fields the user selects for the Folder and File resources
- Twitter: Fixed a typo in the description
- Webhook: Fixed logic for static route matching
- Added the functionality to sort the values that you add in the IF node, Rename node, and the Set node
- Added the functionality to optionally save execution data after each node
- Added queue mode to scale workflow execution
- Separated webhook from the core to scale webhook separately
- Fixed an issue with current execution query for unsaved running workflows
- Fixed an issue with the regex that detected node names
- n8n now generates a unified execution ID instead of two separate IDs for currently running and saved executions

## n8n@0.107.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.106.0...n8n@0.107.0) for this version.<br />
**Release date:** 2021-02-08

- New nodes
- AWS Comprehend
- GetResponse Trigger
- Peekalink
- Stackby
- Enhanced nodes
- AWS SES: Added Custom Verification Email resource
- Microsoft Teams: Added Task resource
- Twitter: Added Delete operation to the Tweet resource
- Bug fixes
- Google Drive: Fixed an issue with the Delete and Share operations
- FileMaker: Fixed an issue with the script list parsing
- Updated Node.js version of Docker images to `14.15`
- Added a shortcut `CTRL + scroll` to zoom

## n8n@0.106.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.105.0...n8n@0.106.0) for this version.<br />
**Release date:** 2021-02-05

- New nodes
- Reddit
- Tapfiliate
- Enhanced nodes
- Airtable Trigger: Added Download Attachment option
- HubSpot: Added Custom Properties option to the Create and Update operations of the Company resource
- MySQL: Added Connection Timeout parameter to the credentials
- Telegram: Added Pin Chat Message and Unpin Chat Message operations for the Message resource
- Bug fixes
- Typeform: Fixed an issue with the OAuth2 authentication method
- Added support for `s` and `u` flags for regex in the IF node and the Switch node

## n8n@0.105.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.104.2...n8n@0.105.0) for this version.<br />
**Release date:** 2021-02-01

- New nodes
- Discourse
- SecurityScorecard
- TimescaleDB
- Enhanced nodes
- Affinity: Added List and List Entry resource
- Asana: Added Project IDs option to the Create operation of the Task resource
- HubSpot Trigger: Added support for multiple subscriptions
- Jira: Added Issue Attachment resource and added custom fields to Create and Update operations of the Issue resource
- Todoist: Added Section option
- Bug fixes
- SIGNL4: Fixed an issue with the attachment functionality
- Added variable `$mode` to check the mode in which the workflow is being executed


## n8n@0.104.2
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.104.1...n8n@0.104.2) for this version.<br />
**Release date:** 2021-01-27

- Fixed an issue with the credentials parameters that have the same name

## n8n@0.104.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.104.0...n8n@0.104.1) for this version.<br />
**Release date:** 2021-01-26

- Fixed a bug with expressions in credentials

## n8n@0.104.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.103.1...n8n@0.104.0) for this version.<br />
**Release date:** 2021-01-26

- New nodes
- Compression
- Enhanced nodes
- GitHub: Added Invite operation to the User resource
- EmailReadImap: Increased the authentication timeout
- Mautic: Added Custom Fields option to the Create and Update operations of the Contact resource. Also, the Mautic OAuth credentials have been updated. Now you don't have to enter the Authorization URL and the Access Token URL
- Nextcloud: Added User resource
- Slack: Added Get Permalink and Delete operations to the Message resource
- Webhook: Added support for request parameters in webhook paths
- Bug fixes
- Google Drive: Fixed the default value for the Send Notification Email option
- Added support for expressions to credentials
- Removed support for MongoDB as a database for n8n. For more details, check out the entry in the [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01040) page

## n8n@0.103.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.103.0...n8n@0.103.1) for this version.<br />
**Release date:** 2021-01-21

- Bug fixes
- Trello: Fixed the icon

## n8n@0.103.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.102.0...n8n@0.103.0) for this version.<br />
**Release date:** 2021-01-21

- New nodes
- SendGrid
- Enhanced nodes
- AMQP: Added Container ID, Reconnect, and Reconnect limit options
- AMQP Trigger: Added Container ID, Reconnect, and Reconnect Limit options
- GitHub: Added Review resource
- Google Drive: Added Drive resource
- Trello: Added Get All and Get Cards operation to the List resource
- Bug fixes
- AWS Lambda: Fixed an issue with signature
- AWS SNS: Fixed an issue with signature
- Fixed an issue with nodes not executing if two input gets passed and one of them didn't return any data
- The code editor doesn'tget closed when clicked anywhere outside the editor
- Added CLI commands to [export](/hosting/cli-commands/#export-workflows-and-credentials) and [import](/hosting/cli-commands/#import-workflows-and-credentials) credentials and workflows
- The title in the browser tab now resets for new workflows


## n8n@0.102.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.101.0...n8n@0.102.0) for this version.<br />
**Release date:** 2021-01-15

- New nodes
- Beeminder
- Enhanced nodes
- Crypto: Added hash type `SHA384`
- Google Books: Added support for user impersonation
- Google Drive: Added support for user impersonation
- Google Sheets: Added support for user impersonation
- Gmail: Added support for user impersonation
- Microsoft Outlook: Added support for a shared mailbox
- RabbitMQ: Added Exchange mode
- Salesforce: Added filters to all Get All operations
- Slack: Made changes to the properties `As User` and `Ephemeral`. For more details, check out the entry in the [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01020) page
- Typeform Trigger: The node now displays the recall information in the question in square brackets. For more details, check out the entry in the [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#01020) page
- Zendesk: Removed the `Authorization URL` and `Access Token URL` fields from the OAuth2 credentials. The node now uses the subdomain passed by a user to connect to Zendesk.
- Bug fixes
- CoinGecko: Fixed an issue to process multiple input items correctly

## n8n@0.101.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.100.0...n8n@0.101.0) for this version.<br />
**Release date:** 2021-01-07

- New nodes
- Google Analytics
- PhantomBuster
- Enhanced nodes
- AWS: Added support for custom endpoints
- Gmail: Added an option to send messages formatted as HTML
- Philips Hue: Added Room/Group name to Light name to make it easier to identify lights
- Slack: Added ephemeral message option
- Telegram: Removed the Bot resource as the endpoint is no longer supported
- Bug fixes
- E-goi: Fixed the name of the node
- Edit Image: Fixed an issue with the Border operation
- HTTP Request: Fixed batch sizing to work when `batchSize = 1`
- PayPal: Fixed a typo in the Environment field
- Split In Batches: Fixed a typo in the description
- Telegram: Fixed an issue with the Send Audio operation
- Based on your settings, vacuum runs on SQLite on startup
- Updated Axios to version `0.21.1`

## n8n@0.100.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.99.1...n8n@0.100.0) for this version.<br />
**Release date:** 2020-12-30

- New nodes
- Microsoft Outlook
- Enhanced nodes
- ActiveCampaign: The node loads more options for the fields
- Asana: Added Subtask resource and Get All operation for the Task resource
- Edit Image: Added Multi Step operation
- HTTP Request: Added Use Querystring option
- IF: Added Ends With and Starts With operations
- Jira: Added Issue Comment resource
- Switch: Added Ends With and Starts With operations
- Telegram: Added File resource
- Bug fixes
- Box Trigger: Fixed a typo in the description
- Edit Image: Fixed an issue with multiple composite operations
- HTTP Request: Fixed an issue with the binary data getting used by multiple nodes
- S3: Fixed an issue with uploading files
- Stripe Trigger: Fixed an issue with the existing webhooks
- Telegram: Fixed an issue with the Send Audio operation
- Binary data stays visible if a node gets re-executed

## n8n@0.99.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.99.0...n8n@0.99.1) for this version.<br />
**Release date:** 2020-12-24

- Fixed a bug that caused HTML to render in JSON view

## n8n@0.99.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.98.0...n8n@0.99.0) for this version.<br />
**Release date:** 2020-12-24

- New nodes
- e-goi
- RabbitMQ
- RabbitMQ Trigger
- uProc
- Enhanced nodes
- ActiveCampaign: Added the functionality to load the tags for a user
- FTP: Added Delete and Rename operation
- Google Cloud Firestore: The node now gives the Collection ID in response
- Iterable: Added User List resource
- MessageBird: Added Balance resource
- TheHive Trigger: Added support for the TheHive3 webhook events, and added Log Updated and Log Deleted events
- Bug fixes
- Dropbox: Fixed an issue with the OAuth credentials
- Google Sheets: Fixed an issue with the parameters getting hidden for other operations
- Added functionality to copy the data and the path from the output
- Fixed an issue with the node getting selected after it was duplicated

## n8n@0.98.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.97.0...n8n@0.98.0) for this version.<br />
**Release date:** 2020-12-16

- New nodes
- Brandfetch
- Pushcut
- Pushcut Trigger
- Enhanced nodes
- Google Sheets: Added Spreadsheet resource
- IF: Added Is Empty option
- Slack: Added Reaction and User resource, and Member operation to the Channel resource
- Spreadsheet File: Added the option Include Empty Cell to display empty cells
- Webhook: Added option to send a custom response body. The node can now also return string data
- Bug fixes
- GitLab: Fixed an issue with GitLab OAuth credentials. You can now specify your GitLab server to configure the credentials
- Mautic: Fixed an issue with the OAuth credentials
- If a workflow is using the Error Trigger node, by default, the workflow will use itself as the Error Workflow
- Fixed a bug that caused the Editor UI to display an incorrect (save) state upon activating or deactivating a workflow
## n8n@0.97.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.96.0...n8n@0.97.0) for this version.<br />
**Release date:** 2020-12-10

- New nodes
- Ghost
- NASA
- Snowflake
- Twist
- Enhanced nodes
- Automizy: Added options to add and remove tabs for the Update operation of the Contact resource
- Pipedrive: Added label field to Person, Organization, and Deal resources. Also added Update operation for the Organization resource
- Bug fixes
- Fixed a bug that caused OAuth1 requests to break
- Fixed Docker user mount path

## n8n@0.96.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.95.1...n8n@0.96.0) for this version.<br />
**Release date:** 2020-12-03

- New nodes
- Cortex
- Iterable
- Kafka Trigger
- TheHive
- TheHive Trigger
- Yourls
- Enhanced nodes
- HubSpot: Added Contact List resource and Search operation for the Deal resource
- Google Calendar: You can now add multiple attendees in the Attendees field
- Slack: The node now loads both private and public channels
- Bug Fixes
- MQTT: Fixed an issue with the connection. The node now uses `mqtt@4.2.1`
- Fixed a bug which caused the Trigger-Nodes to require data from the first output
- Added configuration to load only specific nodes

## n8n@0.95.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.95.0...n8n@0.95.1) for this version.<br />
**Release date:** 2020-11-25

- Bug Fixes
- Airtable Trigger: Fixed the icon of the node

## n8n@0.95.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.94.1...n8n@0.95.0) for this version.<br />
**Release date:** 2020-11-25

- New nodes
- Airtable Trigger
- LingvaNex
- OpenThesaurus
- ProfitWell
- Quick Base
- Spontit
- Enhanced nodes
- Airtable: The Application ID field has been renamed to Base ID, and the Table ID field has been renamed to Table. The List operation now downloads attachments automatically
- Harvest: Moved the account field from the credentials to the node parameters. For more details, check out the entry in the [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#0950) page
- Bug Fixes
- Slack: Fixed an issue with creating channels and inviting users to a channel

## n8n@0.94.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.94.0...n8n@0.94.1) for this version.<br />
**Release date:** 2020-11-20

- Bug Fixes
- GraphQL: Fixed an issue with the variables
- WooCommerce Trigger: Fixed an issue with the webhook. The node now reuses a webhook if it already exists.

## n8n@0.94.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.93.0...n8n@0.94.0) for this version.<br />
**Release date:** 2020-11-19

- New nodes
- Google Cloud Natural Language
- Google Firebase Cloud Firestore
- Google Firebase Realtime Database
- Humantic AI
- Enhanced nodes
- ActiveCampaign: Added Contact List and List resource
- Edit Image: Added support for drawing, font selection, creating a new image, and added the Composite resource
- FTP: Added Private Key and Passphrase fields to the SFTP credentials and made the directory creation more robust
- IMAP: Increased the timeout
- Matrix: Added option to send notice, emote, and HTML messages
- Segment: Made changes to the properties `traits` and `properties`. For more details, check out the entry in the [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#0940) page
- Bug Fixes
- GraphQL: Fixed an issue with the variables
- Mailchimp: Fixed an issue with the OAuth credentials. The credentials are now sent with the body instead of the header
- YouTube: Fixed a typo for the Unlisted option
- Added horizontal scrolling

## n8n@0.93.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.92.0...n8n@0.93.0) for this version.<br />
**Release date:** 2020-11-11

- New nodes
- GetResponse
- Gotify
- Line
- Strapi
- Enhanced nodes
- AMQP: Connection is now closed after a message is sent
- AMQP Trigger: Added Message per Cycle option to retrieve the specified number of messages from the bus for every cycle
- HubSpot: Added Custom Properties for the Deal resource as Additional Fields
- Jira: The node retrieves all the projects for the Project field instead of just 50
- Mattermost: Improved the channel selection
- Microsoft SQL: Added TLS parameter for the credentials
- Pipedrive Trigger: Added OAuth authentication method. For more details, check out the entry in the [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#0930) page
- Segment: Added Custom Traits option for the Traits field
- Bug Fixes
- Shopify Trigger: Fixed an issue with activating the workflow
- For custom nodes, you can now set custom documentation URLs

## n8n@0.92.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.91.0...n8n@0.92.0) for this version.<br />
**Release date:** 2020-11-04

- New nodes
- Facebook Trigger
- Google Books
- Orbit
- Storyblok
- Enhanced nodes
- Google Drive: Removed duplicate parameters
- Twitter: Added Direct Message resource
- Bug Fixes
- Gmail: Fixed an issue with the encoding for the subject field
- Improved the Editor UI for the save workflow functionality

## n8n@0.91.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.90.0...n8n@0.91.0) for this version.<br />
**Release date:** 2020-10-23

- New nodes
- Kafka
- MailerLite
- MailerLite Trigger
- Pushbullet
- Enhanced nodes
- Airtable: Added Ignore Fields option for the Update operation
- AMQP Sender: Added Azure Service Bus support
- Google Calendar: Added Calendar resource and an option to add a conference link
- G Suite Admin: Added Group resource
- HTTP Request: Added Batch Size and Batch Interval option
- Mautic: Added Company resource
- Salesforce: Added OAuth 2.0 JWT authentication method
- Bug Fixes
- IF: Fixed an issue with undefined expression
- Paddle: Fixed an issue with the Return All parameter
- Switch: Fixed an issue with undefined expression
- Added CLI commands to deactivate the workflow
- Added an option to get the full execution data from the server
- The Editor UI gives an alert if you redirect without saving a workflow
- The Editor UI now indicates if a workflow is saved or not
- Improved support for touch devices
- Node properties now load on demand
- Updated the Node.js version for the Docker images


## n8n@0.90.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.89.2...n8n@0.90.0) for this version.<br />
**Release date:** 2020-10-23

- Added a check for the Node.js version on startup. For more details, check out the entry in the [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#0900) page
- Bug Fixes
- Google Translate: Fixed an issue with the rendering of the image in n8n.io

## n8n@0.89.2
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.89.1...n8n@0.89.2) for this version.<br />
**Release date:** 2020-10-22

- Bug Fixes
- Strava Trigger: Fixed a typo in the node name

## n8n@0.89.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.89.0...n8n@0.89.1) for this version.<br />
**Release date:** 2020-10-22

- Removed debug messages

## n8n@0.89.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.88.1...n8n@0.89.0) for this version.<br />
**Release date:** 2020-10-22

- New Nodes
- Pushover
- Strava
- Strava Trigger
- Google Translate
- Bug Fixes
- HTTP Request: Fixed an issue with the POST request method for the 'File' response format
- Fixed issue with displaying non-active workflows as active
- Fixed an issue related to multiple-webhooks

## n8n@0.88.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.88.0...n8n@0.88.1) for this version.<br />
**Release date:** 2020-10-16

- Bug Fixes
- HTTP Request: Fixed an issue with the Form-Data Multipart and the RAW/Custom Body Content Types

## n8n@0.88.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.87.2...n8n@0.88.0) for this version.<br />
**Release date:** 2020-10-16

- Enhanced Fixes
- Matrix: Added support for specifying a Matrix Homeserver URL
- Salesforce: Added Custom Object resource and Custom Fields and Sort options
- Bug Fixes
- AWS SES: Fixed an issue with the Send Template operation for the Email resource
- AWS SNS Trigger: Fixed an issue with the Subscriptions topic

## n8n@0.87.2
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.87.1...n8n@0.87.2) for this version.<br />
**Release date:** 2020-10-15

- Bug Fixes
- Google Sheets: Fixed an issue with spaces in sheet names
- Automizy: Fixed an issue with the default resource

## n8n@0.87.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.87.0...n8n@0.87.1) for this version.<br />
**Release date:** 2020-10-15

- Bug Fixes
- Gmail: Fixed an issue with the Message ID
- HTTP Request: Fixed an issue with the GET Request
- Added `HMAC-SHA512` signature method for OAuth 1.0

## n8n@0.87.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.86.1...n8n@0.87.0) for this version.<br />
**Release date:** 2020-10-14

- New nodes
- Automizy
- AWS Rekognition
- Matrix
- Sendy
- Vonage
- WeKan
- Enhanced nodes
- AWS SES: Added Send Template operation for the Email resource and added the Template resource
- ClickUp: Added Time Entry and Time Entry Tag resources
- Function: The Function field is now called the JavaScript Code field
- Mailchimp: Added Campaign resource
- Mindee: Added currency to the simplified response
- OneDrive: Added Share operation
- OpenWeatherMap: Added Language parameter
- Pipedrive: Added additional parameters to the Get All operation for the Note resource
- Salesforce: Added Flow resource
- Spreadsheet File: Added Range option for the Read from file operation
- Bug Fixes
- ClickUp Trigger: Fixed issue with creating credentials
- Pipedrive Trigger: Fixed issue with adding multiple webhooks to Pipedrive
- The link.fish Scrape node has been removed from n8n. For more details, check out the entry in the [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#0870) page

## n8n@0.86.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.86.0...n8n@0.86.1) for this version.<br />
**Release date:** 2020-10-06

- Enhanced nodes
- CoinGecko: Small fixes to the CoinGecko node

## n8n@0.86.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.85.0...n8n@0.86.0) for this version.<br />
**Release date:** 2020-10-05

- New nodes
- Clockify
- CoinGecko
- G Suite Admin
- Mindee
- Wufoo Trigger
- Enhanced nodes
- Slack: Added User Profile resource
- Mattermost: Added Create and Invite operations for the User resource
- Bug Fixes
- S3: Fixed issue with uploading files
- Webhook ID gets refreshed on node duplication

## n8n@0.85.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.84.4...n8n@0.85.0) for this version.<br />
**Release date:** 2020-09-30

- Enhanced nodes
- Postgres: Added Schema parameter for the Update operation
- Bug Fixes
- Jira: Fixed a bug with the Issue Type field
- Pipedrive Trigger: Fixed issues with the credentials
- Changed the bcrypt library to `bcrypt.js` to make it compatible with Windows
- The OAuth callback URLs are now generated in the backend

## n8n@0.84.4
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.84.3...n8n@0.84.4) for this version.<br />
**Release date:** 2020-09-23

- Bug Fixes
- Google Sheets: Fixed issues with the update and append operations

## n8n@0.84.3
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.84.2...n8n@0.84.3) for this version.<br />
**Release date:** 2020-09-23

- Fixed an issue with the build by setting `jwks-rsa` to an older version

## n8n@0.84.2
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.84.1...n8n@0.84.2) for this version.<br />
**Release date:** 2020-09-23

- Fixed an issue with the OAuth window. The OAuth window now closes after authentication is complete

## n8n@0.84.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.84.0...n8n@0.84.1) for this version.<br />
**Release date:** 2020-09-23

- Additional endpoints can be excluded from authentication checks. Multiple endpoints can be added separated by colons

## n8n@0.84.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.83.0...n8n@0.84.0) for this version.<br />
**Release date:** 2020-09-23

- Enhanced nodes
- Twitter: Added support for auto mention of users in reply tweets
- Bug Fixes
- Google Sheets: Fixed issue with non-Latin sheet names
- HubSpot: Fixed naming of credentials
- Microsoft: Fixed naming of credentials
- Mandrill: Fixed attachments with JSON parameters
- Expressions now use short variables when selecting input data for the current node
- Fixed issue with renaming credentials for active workflows

## n8n@0.83.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.82.1...n8n@0.83.0) for this version.<br />
**Release date:** 2020-09-18

- New nodes
- LinkedIn
- Taiga
- Taiga Trigger
- Enhanced nodes
- ActiveCampaign: Added multiple functions, read more [here](https://github.com/n8n-io/n8n/commit/a552febab494f8ecc022391f046752f1f9f5a4cc)
- Airtable: Added typecast functionality
- Asana: Added OAuth2 support
- ClickUp: Added OAuth2 support
- Google Drive: Added share operation
- IMAP Email: Added support for custom rules when checking emails
- Sentry.io: Added support for self-hosted version
- Twitter: Added retweet, reply, and like operations
- WordPress: Added author field to the post resource
- Bug Fixes
- Asana Trigger: Webhook validation has been deactivated
- Paddle: Fixed `returnData` format and coupon description
- The ActiveCampaign node has [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#0830)
- Fixed issues with test-webhook registration

## n8n@0.82.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.82.0...n8n@0.82.1) for this version.<br />
**Release date:** 2020-09-14

- Speed for basic authentication with hashed password has been improved

## n8n@0.82.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.81.0...n8n@0.82.0) for this version.<br />
**Release date:** 2020-09-14

- New nodes
- Microsoft Teams
- Enhanced nodes
- Freshdesk: Added Freshdesk contact resource
- HTTP Request: Run parallel requests in HTTP Request Node
- Bug Fixes
- Philips Hue: Added `APP ID` to Philips Hue node credentials
- Postmark Trigger: Fixed parameters for the node
- The default space between nodes has been increased to two units
- Expression support has been added to the credentials
- Passwords for your n8n instance can now be hashed

## n8n@0.81.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.80.0...n8n@0.81.0) for this version.<br />
**Release date:** 2020-09-09

- New nodes
- Sentry.io
- Enhanced nodes
- Asana
- ClickUp
- Clockify
- Google Contacts
- Salesforce
- Segment
- Telegram
- Telegram Trigger

## n8n@0.80.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.79.0...n8n@0.80.0) for this version.<br />
**Release date:** 2020-09-02

- New nodes
- Customer.io
- MQTT Trigger
- S3
- Enhanced nodes
- Acuity Scheduling
- AWS S3
- ClickUp
- FTP
- Telegram Trigger
- Zendesk

## n8n@0.79.3
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.79.2...n8n@0.79.3) for this version.<br />
**Release date:** 2020-08-30

- The bug that caused the workflows to not get activated correctly has been fixed

## n8n@0.79.2
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.79.1...n8n@0.79.2) for this version.<br />
**Release date:** 2020-08-28

- Added missing rawBody for "application/x-www-form-urlencoded"

## n8n@0.79.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.79.0...n8n@0.79.1) for this version.<br />
**Release date:** 2020-08-28

- Enhanced nodes
- Contentful
- HTTP Request
- Postgres
- Webhook
- Removed Test-Webhook also in case checkExists fails
- HTTP Request node doesn'toverwrite accept header if it's already set
- Add rawBody to every request so that n8n doesn'tgive an error if body is missing

## n8n@0.79.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.79.2...n8n@0.79.3) for this version.<br />
**Release date:** 2020-08-27

- New nodes
- Contentful
- ConvertKit
- ConvertKit Trigger
- Paddle
- Enhanced nodes
- Airtable
- Coda
- Gmail
- HubSpot
- IMAP Email
- Postgres
- Salesforce
- SIGNL4
- Todoist
- Trello
- YouTube
- The Todoist node has [breaking changes](https://github.com/n8n-io/n8n/blob/master/packages/cli/BREAKING-CHANGES.md#0790)
- Added dynamic titles on workflow execution
- Nodes will now display a link to associated credential documentation

## n8n@0.78.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.76.0...n8n@0.78.0) for this version.<br />
**Release date:** 2020-08-18

- New nodes
- Gmail
- Google Contacts
- Unleashed Software
- YouTube
- Enhanced nodes
- AMQP
- AMQP Trigger
- Bitly
- Function Item
- Google Sheets
- Shopify
- Todoist
- Enhanced support for [JWT based authentication](/hosting/authentication/jwt/)
- Added an option to execute a node once, using data of only the first item

## n8n@0.76.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.75.0...n8n@0.76.0) for this version.<br />
**Release date:** 2020-08-05

- New nodes
- Customer.io Trigger
- FTP
- Medium
- Philips Hue
- TravisCI
- Twake
- Enhanced nodes
- CrateDB
- Move Binary Data
- Nodes will now display a link to associated documentation

## n8n@0.75.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.74.0...n8n@0.75.0) for this version.<br />
**Release date:** 2020-07-26

- New nodes
- Box
- Box Trigger
- CrateDB
- Jira Trigger
- Enhanced nodes
- GitLab
- Nextcloud
- Pipedrive
- QuestDB
- Webhooks now support OPTIONS request

## n8n@0.74.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.73.1...n8n@0.74.0) for this version.<br />
**Release date:** 2020-07-15

- New nodes
- Hacker News
- QuestDB
- Xero
- Enhanced nodes
- Affinity Trigger
- HTTP Request
- Mailchimp
- MongoDB
- Pipedrive
- Postgres
- UpLead
- Webhook
- Webhook URLs are now handled independently of the workflow ID by `https://{hostname}/webhook/{path}` instead of the older `https://{hostname}/webhook/{workflow_id}/{node_name}/{path}`.


## n8n@0.73.1
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.73.0...n8n@0.73.1) for this version.<br />
**Release date:** 2020-07-08

- Enhanced nodes
- Microsoft SQL


## n8n@0.73.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.72.0...n8n@0.73.0) for this version.<br />
**Release date:** 2020-07-08

- New nodes
- CircleCI
- Microsoft SQL
- Zoom
- Enhanced nodes
- Postmark Trigger
- Salesforce
- It's now possible to set default values for credentials that get prefilled, and the user can't change.


## n8n@0.72.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.71.0...n8n@0.72.0) for this version.<br />
**Release date:** 2020-07-02

- Enhanced nodes
- Drift
- Eventbrite Trigger
- Facebook Graph API
- Pipedrive
- Fixed credential issue for the Execute Workflow node


## n8n@0.71.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.70.0...n8n@0.71.0) for this version.<br />
**Release date:** 2020-06-25

- New nodes
- Google Tasks
- SIGNL4
- Spotify
- Enhanced nodes
- HubSpot
- Mailchimp
- Typeform
- Webflow
- Zendesk
- Added Postgres SSL support
- It's now possible to deploy n8n under a subfolder


## n8n@0.70.0
For a comprehensive list of changes, check out the [commits](https://github.com/n8n-io/n8n/compare/n8n@0.69.1...n8n@0.70.0) for this version.<br />
**Release date:** 2020-06-13

- Enhanced nodes
- GitHub
- Mautic Trigger
- Monday.com
- MongoDB
- Fixed the issue with multiuser-setup

<!-- vale on -->
