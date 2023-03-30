---
title: AWS Rekognition
description: Documentation for the AWS Rekognition node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

# AWS Rekognition

The AWS Rekognition node allows you to automate work in AWS Rekognition, and integrate AWS Rekognition with other applications. n8n has built-in support for a wide range of AWS Rekognition features, including analyzing images.

On this page, you'll find a list of operations the AWS Rekognition node supports and links to more resources.

!!! note "Credentials"
    Refer to [AWS Rekognition credentials](/integrations/builtin/credentials/aws/) for guidance on setting up authentication. 

!!! note "Examples and Templates"
    For usage examples and templates to help you get started, take a look at n8n's [AWS Rekognition integrations](https://n8n.io/integrations/aws-rekognition/){:target=_blank .external-link} list.



## Basic Operations

**Image**

- Analyze


## Example Usage

This workflow allows you to detect a face from an image using the AWS Rekognition node. You can also find the [workflow](https://n8n.io/workflows/694) on n8n.io. This example usage workflow uses the following nodes.
- [Start](/integrations/builtin/core-nodes/n8n-nodes-base.start/)
- [HTTP Request](/integrations/builtin/core-nodes/n8n-nodes-base.httprequest/)
- [AWS Rekognition]()

The final workflow should look like the following image.

![A workflow with the AWS Rekognition node](/_images/integrations/builtin/app-nodes/awsrekognition/workflow.png)

### 1. Start node

The Start node exists by default when you create a new workflow.


### 2. HTTP Request node (GET)

This example workflow uses the HTTP Request node to fetch an image from a URL. You can also use the [Read Binary File](/integrations/builtin/core-nodes/n8n-nodes-base.readbinaryfile/) node to read an image file from the path you specify.

1. Enter the URL of the image in the ***URL*** field. For example, `https://n8n.io/_nuxt/img/04c67e5.png`.
2. Select 'File' from the ***Response Format*** dropdown list.
3. Click on ***Execute Node*** to run the node.

In the screenshot below, you will notice that the HTTP Request node fetches the image from the URL. This image gets passed on as binary data to the next node in the workflow.

![Using the HTTP Request node to fetch an image from a URL](/_images/integrations/builtin/app-nodes/awsrekognition/httprequest_node.png)


### 3. AWS Rekognition node (analyze: image)

This node will detect faces in the image that we fetched in the previous node. You can also use this node to analyze an image stored in your AWS Bucket.

1. First of all, you'll have to enter credentials for the AWS Rekognition node. You can find out how to enter credentials for this node [here](/integrations/builtin/credentials/aws/).
2. Set ***Binary Data*** to `true`.
3. Click on ***Execute Node*** to run the node.

In the screenshot below, you will observe that the node detects the face in the image that we got from the HTTP Request node.

![Using the AWS Rekognition node to detect faces in an image](/_images/integrations/builtin/app-nodes/awsrekognition/awsrekognition_node.png)

