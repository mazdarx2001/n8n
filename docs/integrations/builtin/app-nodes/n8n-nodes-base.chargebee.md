---
title: Chargebee
description: Documentation for the Chargebee node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

# Chargebee

The Chargebee node allows you to automate work in Chargebee, and integrate Chargebee with other applications. n8n has built-in support for a wide range of Chargebee features, including creating customers, returning invoices, and canceling subscriptions.

On this page, you'll find a list of operations the Chargebee node supports and links to more resources.

!!! note "Credentials"
    Refer to [Chargebee credentials](/integrations/builtin/credentials/chargebee/) for guidance on setting up authentication. 

!!! note "Examples and Templates"
    For usage examples and templates to help you get started, take a look at n8n's [Chargebee integrations](https://n8n.io/integrations/chargebee/){:target=_blank .external-link} list.




## Basic Operations

* Customer
    * Create a customer
* Invoice
    * Return the invoices
    * Get URL for the invoice PDF
* Subscription
    * Cancel a subscription
    * Delete a subscription

## Example Usage

This workflow allows you to create a new customer in Chargebee. You can also find the [workflow](https://n8n.io/workflows/483) on the website. This example usage workflow would use the following two nodes.
- [Start](/integrations/builtin/core-nodes/n8n-nodes-base.start/)
- [Chargebee]()

The final workflow should look like the following image.

![A workflow with the Chargebee node](/_images/integrations/builtin/app-nodes/chargebee/workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.

### 2. Chargebee node

1. First of all, you'll have to enter credentials for the Chargebee node. You can find out how to do that [here](/integrations/builtin/credentials/chargebee/).
2. Select the 'Customer' option from the *Resource* dropdown list.
3. Under the *Properties* section, click on the *Add Property* button and select *First Name*.
5. Enter the first name of the contact in the *First Name* field.
6. Click on *Add Property* again and select *Last Name*.
7. Enter the last name of the contact in the *Last name* field.
8. Click on *Execute Node* to run the workflow.

