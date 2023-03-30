---
title: Trello
description: Documentation for the Trello node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

# Trello

The Trello node allows you to automate work in Trello, and integrate Trello with other applications. n8n has built-in support for a wide range of Trello features, including creating and updating cards, and adding and removing members. 

On this page, you'll find a list of operations the Trello node supports and links to more resources.

!!! note "Credentials"
    Refer to [Trello credentials](/integrations/builtin/credentials/trello/) for guidance on setting up authentication. 

!!! note "Examples and templates"
    For usage examples and templates to help you get started, take a look at n8n's [Trello integrations](https://n8n.io/integrations/trello/){:target="_blank" .external-link} list.


## Basic Operations

* Attachment
    * Create a new attachment for a card
    * Delete an attachment
    * Get the data of an attachment
    * Returns all attachments for the card
* Board
    * Create a new board
    * Delete a board
    * Get the data of a board
    * Update a board
* Board Member
    * Add
    * Get All
    * Invite
    * Remove
* Card
    * Create a new card
    * Delete a card
    * Get the data of a card
    * Update a card
* Card Comment
    * Create a comment on a card
    * Delete a comment from a card
    * Update a comment on a card
* Checklist
    * Create a checklist item
    * Create a new checklist
    * Delete a checklist
    * Delete a checklist item
    * Get the data of a checklist
    * Returns all checklists for the card
    * Get a specific checklist on a card
    * Get the completed checklist items on a card
    * Update an item in a checklist on a card
* Label
    * Add a label to a card.
    * Create a new label
    * Delete a label
    * Get the data of a label
    * Returns all labels for the board
    * Remove a label from a card.
    * Update a label.
* List
    * Archive/Unarchive a list
    * Create a new list
    * Get the data of a list
    * Get all the lists
    * Get all the cards in a list
    * Update a list

## Example Usage

This workflow allows you to create a new card in Trello. You can also find the [workflow](https://n8n.io/workflows/461) on the website. This example usage workflow would use the following two nodes.
- [Start](/integrations/builtin/core-nodes/n8n-nodes-base.start/)
- [Trello]()

The final workflow should look like the following image.

![A workflow with the Trello node](/_images/integrations/builtin/app-nodes/trello/workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.

### 2. Trello node

1. First of all, you'll have to enter credentials for the Trello node. You can find out how to do that [here](/integrations/builtin/credentials/trello/).
2. Enter the ID of the list in which you want to create a new card in the *List ID* field. You can find instructions on how to obtain the ID of the list in the FAQs below.
3. Enter the name of the card in the *Name* field.
4. Enter the description of the card in the *Description* field.
5. Click on *Execute Node* to run the workflow.


## FAQs

### How do I find the List ID?

1. Open the Trello board that contains the list.
2. If the list doesn't have any cards, add a card to the list.
3. Open the card, add '.json' at the end of the URL, and press enter.
4. In the JSON file, you will see a field called `idList`.
5. Copy `idList`and paste it in the *List ID* field in n8n.






