---
permalink: /nodes/n8n-nodes-base.stripeTrigger
---

# Stripe Trigger

Stripe is a suite of payment APIs that powers commerce for online businesses.

::: tip 🔑 Credentials
You can find authentication information for this node [here](../../../credentials/Stripe/README.md).
:::


## Example Usage

This workflow allows you to receive updates for Stripe events. You can also find the [workflow](https://n8n.io/workflows/545) on the website. This example usage workflow would use the following node.
- [Stripe Trigger]()

The final workflow should look like the following image.

![A workflow with the Stripe Trigger node](./workflow.png)


### 1. Stripe Trigger node

1. First of all, you'll have to enter credentials for the Stripe Trigger node. You can find out how to do that [here](../../../credentials/Stripe/README.md).
2. Select the `*` option in the *Events* field to receive updates when any event is triggered.
3. Click on *Execute Node* to run the workflow.
