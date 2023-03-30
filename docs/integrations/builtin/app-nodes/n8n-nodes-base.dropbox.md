---
title: Dropbox
description: Documentation for the Dropbox node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

# Dropbox

The Dropbox node allows you to automate work in Dropbox, and integrate Dropbox with other applications. n8n has built-in support for a wide range of Dropbox features, including creating, downloading, moving, and copying files and folders.

On this page, you'll find a list of operations the Dropbox node supports and links to more resources.

!!! note "Credentials"
    Refer to [Dropbox credentials](/integrations/builtin/credentials/dropbox/) for guidance on setting up authentication. 

!!! note "Examples and templates"
    For usage examples and templates to help you get started, take a look at n8n's [Dropbox integrations](https://n8n.io/integrations/dropbox/){:target="_blank" .external-link} list.


## Basic Operations

* File
    * Copy a file
    * Delete a file
    * Download a file
    * Move a file
    * Upload a file
* Folder
    * Copy a folder
    * Create a folder
    * Delete a folder
    * Return the files and folders in a given folder
    * Move a folder
* Search
    * Query

## Example Usage

This workflow allows you to create a folder in Dropbox, upload a file into that folder, and list the contents of the folder. You can also find the [workflow](https://n8n.io/workflows/615) on n8n.io. This example usage workflow uses the following nodes.
- [Start](/integrations/builtin/core-nodes/n8n-nodes-base.start/)
- [Dropbox]()
- [HTTP Request](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/)

The final workflow should look like the following image.

![A workflow with the Dropbox node](/_images/integrations/builtin/app-nodes/dropbox/workflow.png)

### 1. Start node

The Start node exists by default when you create a new workflow.

### 2. Dropbox node (create: folder)

1. First of all, you'll have to enter credentials for the Dropbox node. You can find out how to do that [here](/integrations/builtin/credentials/dropbox/).
2. Select 'Folder' from the ***Resource*** dropdown list.
3. Enter the name of the new folder in the ***Folder*** field.
4. Click on ***Execute Node*** to run the workflow.

![Create a folder in Dropbox using the Dropbox node](/_images/integrations/builtin/app-nodes/dropbox/dropbox_node.png)

### 3. HTTP Request node (GET)

1. Enter `https://n8n.io/n8n-logo.png` in the ***URL*** field.
2. Select 'File' from the ***Response Format*** dropdown list.
3. Click on ***Execute Node*** to run the workflow.

![Get a file to upload in Dropbox using the HTTP Request node](/_images/integrations/builtin/app-nodes/dropbox/httprequest_node.png)

### 4. Dropbox1 node (upload: file)

1. Select the credentials that you entered in the Dropbox node.
2. Enter the path of the Dropbox folder you created in the previous steps along with a file name in the ***File Path*** field.
3. Set the ***Binary Data*** toggle to true.
4. Click on ***Execute Node*** to run the node.

![Upload a file in Dropbox using the Dropbox node](/_images/integrations/builtin/app-nodes/dropbox/dropbox1_node.png)

### 5. Dropbox2 node (list: folder)

1. Select the credentials that you entered in the Dropbox node.
2. Select 'Folder' from the ***Resource*** dropdown list.
3. Select 'List' from the ***Operation*** dropdown list.
4. Enter the path of the Dropbox folder you created in the previous steps in the ***Folder Path*** field.
5. Click on ***Execute Node*** to run the node.

![List the contents of a Dropbox folder using the Dropbox node](/_images/integrations/builtin/app-nodes/dropbox/dropbox2_node.png)

