---
#https://www.notion.so/n8n/Frontmatter-432c2b8dff1f43d4b1c8d20075510fe4
title: Asana
description: Documentation for the Asana node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
contentType: integration
---

# Asana

Use the Asana node to automate work in Asana, and integrate Asana with other applications. n8n has built-in support for a wide range of Asana features, including creating, updating, deleting, and getting users, tasks, projects, and subtasks.

On this page, you'll find a list of operations the Asana node supports and links to more resources.

/// note | Credentials
Refer to [Asana credentials](/integrations/builtin/credentials/asana/) for guidance on setting up authentication. 
///

/// note | Update to 1.22.2 or above
Due to changes in Asana's API, some operations in this node stopped working on 17th January 2023. Upgrade to n8n 1.22.2 or above.
///

## Operations

* Project
    * Create a new project
    * Delete a project
    * Get a project
    * Get all projects
    * Update a project
* Subtask
    * Create a subtask
    * Get all subtasks
* Task
    * Create a task
    * Delete a task
    * Get a task
    * Get all tasks
    * Move a task
    * Search for tasks
    * Update a task
* Task Comment
    * Add a comment to a task
    * Remove a comment from a task
* Task Tag
    * Add a tag to a task
    * Remove a tag from a task
* Task Project
    * Add a task to a project
    * Remove a task from a project
* User
    * Get a user
    * Get all users

## Templates and examples

<!-- see https://www.notion.so/n8n/Pull-in-templates-for-the-integrations-pages-37c716837b804d30a33b47475f6e3780 -->
[[ templatesWidget(title, 'asana') ]]

--8<-- "_snippets/integrations/builtin/app-nodes/operation-not-supported.md"



