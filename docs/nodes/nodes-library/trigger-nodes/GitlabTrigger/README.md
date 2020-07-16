---
permalink: /nodes/n8n-nodes-base.gitlabTrigger
---

# GitLab Trigger

[GitLab](https://gitlab.com/) is a web-based DevOps lifecycle tool that provides a Git-repository manager providing wiki, issue-tracking and continuous integration/continuous deployment pipeline features, using an open-source license, developed by GitLab Inc.

::: tip 🔑 Credentials
You can find authentication information for this node [here](../../../credentials/Gitlab/README.md).
:::


## Example Usage

This workflow allows you to receive updates for Gitlab events. You can also find the [workflow](https://n8n.io/workflows/528) on the website. This example usage workflow would use the following node.
- [Gitlab Trigger]()

The final workflow should look like the following image.

![A workflow with the Gitlab Trigger node](./workflow.png)


### 1. Gitlab Trigger node

1. First of all, you'll have to enter credentials for the Gitlab Trigger node. You can find out how to do that [here](../../../credentials/Gitlab/README.md).
2. Enter the repository owner in the *Repository Owner* field.
3. Enter the repository name in the *Repository Name* field.
4. Select the events you want to receive updates for from the *Events* dropdown list.
5. Click on *Execute Node* to run the workflow.
