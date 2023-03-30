---
title: Box
description: Documentation for the Box node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

# Box

The Box node allows you to automate work in Box, and integrate Box with other applications. n8n has built-in support for a wide range of Box features, including creating, copying, deleting, searching, uploading, and downloading files and folders.

On this page, you'll find a list of operations the Box node supports and links to more resources.

!!! note "Credentials"
    Refer to [Box credentials](/integrations/builtin/credentials/box/) for guidance on setting up authentication. 

!!! note "Examples and Templates"
    For usage examples and templates to help you get started, take a look at n8n's [Box integrations](https://n8n.io/integrations/box/){:target=_blank .external-link} list.

 

## Basic Operations

* File
    * Copy a file
    * Delete a file
    * Download a file
    * Get a file
    * Search files
    * Share a file
    * Upload a file
* Folder
    * Create a folder
    * Get a folder
    * Delete a folder
    * Search files
    * Share a folder
    * Update folder

## Example Usage

This workflow allows you to create a folder on Box. You can also find the [workflow](https://n8n.io/workflows/559) on the website. This example usage workflow would use the following two nodes.
- [Start](/integrations/builtin/core-nodes/n8n-nodes-base.start/)
- [Box]()

The final workflow should look like the following image.

![A workflow with the Box node](/_images/integrations/builtin/app-nodes/box/workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.

### 2. Box node

1. First of all, you'll have to enter credentials for the Box node. You can find out how to do that [here](/integrations/builtin/credentials/box/).
2. Select the 'Folder' option from the *Resource* dropdown list.
3. Enter the name of the folder in the *Name* field.
4. Click on *Execute Node* to run the workflow.

