---
title: Affinity
description: Documentation for the Affinity node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

# Affinity

The Affinity node allows you to automate work in Affinity, and integrate Affinity with other applications. n8n has built-in support for a wide range of Affinity features, including creating, getting, updating and deleting lists, entries, organization, and persons.

On this page, you'll find a list of operations the Affinity node supports and links to more resources.

!!! note "Credentials"
    Refer to [Affinity credentials](/integrations/builtin/credentials/affinity/) for guidance on setting up authentication.
	
!!! note "Examples and templates"
    For usage examples and templates to help you get started, take a look at n8n's [Affinity integrations](https://n8n.io/integrations/affinity/){:target="_blank" .external-link} list.


## Basic Operations

* List
    * Get a list
    * Get all lists
* List Entry
    * Create a list entry
    * Delete a list entry
    * Get a list entry
    * Get all list entries
* Organization
    * Create an organization
    * Delete an organization
    * Get an organization
    * Get all organizations
    * Update an organization
* Person
    * Create a person
    * Delete a person
    * Get a person
    * Get all persons
    * Update a person


## Example Usage

This workflow allows you to create an organization in Affinity. You can also find the [workflow](https://n8n.io/workflows/476) on the website. This example usage workflow would use the following two nodes.
- [Start](/integrations/builtin/core-nodes/n8n-nodes-base.start/)
- [Affinity]()

The final workflow should look like the following image.

![A workflow with the Affinity node](/_images/integrations/builtin/app-nodes/affinity/workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.

### 2. Affinity node

1. First of all, you'll have to enter credentials for the Affinity node. You can find out how to do that [here](/integrations/builtin/credentials/affinity/).
2. Enter the name of the organization in the *Name* field.
3. Enter the domain name of the organization in the *Domain* field.
4. Click on *Execute Node* to run the workflow.

