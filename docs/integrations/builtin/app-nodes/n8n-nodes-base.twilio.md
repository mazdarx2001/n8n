---
title: Twilio
description: Documentation for the Twilio node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

# Twilio

The Twilio node allows you to automate work in Twilio, and integrate Twilio with other applications. n8n supports sending MMS/SMS and WhatsApp messages with Twilio. 

On this page, you'll find a list of operations the Twilio node supports and links to more resources.

!!! note "Credentials"
    Refer to [Twilio credentials](/integrations/builtin/credentials/twilio/) for guidance on setting up authentication. 

!!! note "Examples and templates"
    For usage examples and templates to help you get started, take a look at n8n's [Twilio integrations](https://n8n.io/integrations/twilio/){:target="_blank" .external-link} list.


## Basic Operations

* SMS
    * Send SMS/MMS/WhatsApp message

## Example Usage

This workflow allows you to send an SMS or a Whatsapp message to a specified phone number from your Twilio number. You can also find the [workflow](https://n8n.io/workflows/401) on the website. This example usage workflow would use the following two nodes.
- [Start](/integrations/builtin/core-nodes/n8n-nodes-base.start/)
- [Twilio]()

The final workflow should look like the following image.

![A workflow with the Twilio node](/_images/integrations/builtin/app-nodes/twilio/workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.

### 2. Twilio node

1. First of all, you'll have to enter credentials for the Twilio node. You can find out how to do that [here](/integrations/builtin/credentials/twilio/).
2. Enter the phone number from which you'll be sending the message in the *From* field.
3. Enter the phone number to which you'll be sending the message in the *To* field.
4. In case you want to send a Whatsapp message, toggle the *To Whatsapp* button.
5. Enter you message in the *Message* field.
6. Click on *Execute Node* to run the workflow.






