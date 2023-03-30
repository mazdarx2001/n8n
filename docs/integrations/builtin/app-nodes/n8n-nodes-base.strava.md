---
title: Strava
description: Documentation for the Strava node in n8n, a workflow automation platform. Includes details of operations and configuration, and links to examples and credentials information.
---

# Strava

The Strava node allows you to automate work in Strava, and integrate Strava with other applications. n8n has built-in support for a wide range of Strava features, including creating new activities, and getting activity information. 

On this page, you'll find a list of operations the Strava node supports and links to more resources.

!!! note "Credentials"
    Refer to [Strava credentials](/integrations/builtin/credentials/strava/) for guidance on setting up authentication. 

!!! note "Examples and templates"
    For usage examples and templates to help you get started, take a look at n8n's [Strava integrations](https://n8n.io/integrations/strava/){:target="_blank" .external-link} list.


## Basic Operations

* Activity
    * Create a new activity
    * Get an activity
    * Get all activities
    * Get all activity comments
    * Get all activity kudos
    * Get all activity laps
    * Get all activity zones
    * Update an activity

## Example Usage

This workflow allows you to create, update, and get an activity in Strava. You can also find the [workflow](https://n8n.io/workflows/744) on n8n.io. This example usage workflow would use the following nodes.
- [Start](/integrations/builtin/core-nodes/n8n-nodes-base.start/)
- [Strava]()

The final workflow should look like the following image.

![A workflow with the Strava node](/_images/integrations/builtin/app-nodes/strava/workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.

### 2. Strava node (create: activity)

This node will create an activity with the name `Morning Run` in Strava. To create an activity with a different name, you can enter the name of your activity instead.

1. First of all, you'll have to enter credentials for the Strava node. You can find out how to do that [here](/integrations/builtin/credentials/strava/).
2. Enter `Morning Run` in the ***Name*** field.
3. Enter `Run` in the ***Type*** field.
4. Select the date and time in the ***Start Date*** field.
5. Set ***Elapsed Time (Seconds)*** to `3600`.
6. Click on the ***Add Field*** button and select 'Distance' from the dropdown list.
7. Set ***Distance*** to `1000`. Strava measures distance in meters.
8. Click on ***Execute Node*** to run the node.

In the screenshot below, you will notice that the node creates an activity with the name `Morning Run` and type `Run`.

![Using the Strava node to create an activity](/_images/integrations/builtin/app-nodes/strava/strava_node.png)



### 3. Strava1 node (update: activity)

This node will update the activity that we created in the previous node.

1. Select the credentials that you entered in the previous node.
2. Select 'Update' from the ***Operation*** dropdown list.
3. Click on the gears icon next to the ***Activity ID*** field and click on ***Add Expression***.
4. Select the following in the ***Variable Selector*** section: Nodes > Strava > Output Data > JSON > id. You can also add the following expression: `{{$node["Strava"].json["id"]}}`.
5. Click on the ***Add Field*** button and select 'Description' from the dropdown list.
6. Enter the description of the activity in the ***Description*** field.
7. Click on ***Execute Node*** to run the node.


In the screenshot below, you will notice that the node adds a description to the activity that we created using the Strava node.

![Using the Strava node to update an activity](/_images/integrations/builtin/app-nodes/strava/strava1_node.png)



### 4. Strava2 node (get: activity)

This node returns the information of the activity that we created using the Strava node.

1. Select the credentials that you entered in the previous node.
2. Select 'Get' from the ***Operation*** dropdown list.
3. Click on the gears icon next to the ***Activity ID*** field and click on ***Add Expression***.
4. Select the following in the ***Variable Selector*** section: Nodes > Strava > Output Data > JSON > id. You can also add the following expression: `{{$node["Strava"].json["id"]}}`.
5. Click on ***Execute Node*** to run the node.


In the screenshot below, you will notice that the node returns the information of the activity that we specified in this node.

![Using the Strava node to get an issue](/_images/integrations/builtin/app-nodes/strava/strava2_node.png)





