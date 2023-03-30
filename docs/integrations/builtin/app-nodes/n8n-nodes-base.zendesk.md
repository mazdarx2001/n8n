---
title: Zendesk
description: Documentation for the Zendesk node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

# Zendesk

The Zendesk node allows you to automate work in Zendesk, and integrate Zendesk with other applications. n8n has built-in support for a wide range of Zendesk features, including creating, and deleting tickets, users, and organizations. 

On this page, you'll find a list of operations the Zendesk node supports and links to more resources.

!!! note "Credentials"
    Refer to [Zendesk credentials](/integrations/builtin/credentials/zendesk/) for guidance on setting up authentication. 

!!! note "Examples and templates"
    For usage examples and templates to help you get started, take a look at n8n's [Zendesk integrations](https://n8n.io/integrations/zendesk/){:target="_blank" .external-link} list.


## Basic Operations

* Ticket
    * Create a ticket
    * Delete a ticket
    * Get a ticket
    * Get all tickets
    * Recover a suspended ticket
    * Update a ticket
* Ticket Field
    * Get a ticket field
    * Get all system and custom ticket fields
* User
    * Create a user
    * Delete a user
    * Get a user
    * Get all users
    * Get a user's organizations
    * Get data related to the user
    * Search users
    * Update a user
* Organization
    * Create an organization
    * Delete an organization
    * Count organizations
    * Get an organization
    * Get all organizations
    * Get data related to the organization
    * Update a organization

## Example Usage

This workflow allows you to create a ticket in Zendesk. You can also find the [workflow](https://n8n.io/workflows/496) on the website. This example usage workflow would use the following two nodes.
- [Start](/integrations/builtin/core-nodes/n8n-nodes-base.start/)
- [Zendesk]()

The final workflow should look like the following image.

![A workflow with the Zendesk node](/_images/integrations/builtin/app-nodes/zendesk/workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.

### 2. Zendesk node

1. First of all, you'll have to enter credentials for the Zendesk node. You can find out how to do that [here](/integrations/builtin/credentials/zendesk/).
2. Enter the description of the ticket in the *Description* field.
3. Click on *Execute Node* to run the workflow.

