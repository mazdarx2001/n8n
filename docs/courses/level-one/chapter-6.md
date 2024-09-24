---
#https://www.notion.so/n8n/Frontmatter-432c2b8dff1f43d4b1c8d20075510fe4
contentType: tutorial
---

# Exporting and importing workflows

In this chapter, you will learn how to export and import workflows.

## Exporting and importing workflows

You can save n8n workflows locally as JSON files. This is useful if you want to share your workflow with someone else or import a workflow from someone else.

--8<-- "_snippets/workflows/sharing-credentials.md"

<figure><img src="/_images/courses/level-one/chapter-six/l1-c6-import-export-menu.png" alt="Import/Export menu" style="width:100%"><figcaption align = "center"><i>Import & Export workflows menu</i></figcaption></figure>

You can export and import workflows in two ways:

* From the **Editor UI**:
    * Export: From the top navigation bar, select the three dots in the upper right, then select **Download**. This will download your current workflow as a JSON file on your computer.
    * Import: From the top navigation bar, select the three dots in the upper right, then select **Import from URL** (to import a published workflow) or **Import from File** (to import a workflow as a JSON file).
* From the command line:
    * Export: See the [full list of commands ](/hosting/cli-commands/){:target="_blank" .external} for exporting workflows or credentials.
    * Import: See the [full list of commands ](/hosting/cli-commands/#import-workflows-and-credentials){:target="_blank" .external} for importing workflows or credentials.

<!--
## Sharing workflows

We love to see what users build with n8n and discover inspiring workflows! On the [n8n workflows page](https://n8n.io/workflows){:target="_blank" .external} you can find hundreds of workflows contributed by our team or community of users.

Since now you know how to build workflows, we encourage you to build more helpful and original workflows and share them with the community.

To share a workflow, follow these steps:

1. Sign in to [n8n.io](https://n8n.io/login){:target="_blank" .external}.
2. Click on the **_+ Share New Workflow_** button.
3. Enter the name of your workflow in the **_Name_** field.
The name should be descriptive for the purpose of the workflow and easy for other users to understand.

4. In the **_Description_** field, add a screenshot of your workflow and write a description below it.
	* The screenshot should capture the entire Editor UI.
	* The description should list all the nodes used in the workflow and the function they serve. You should also mention any prerequisites for building the workflow.

    !!! tip  Workflow description template
        [This is an example](https://n8n.io/workflows/1110){:target="_blank" .external} of a well-written description that you can use as a template for your own workflows.


5. In the Editor UI, select all the nodes in your workflow (Ctrl + A or Cmd + A) and copy them (Ctrl + C or Cmd + C).
6. In the **_Workflow Code_** field, delete the existing code and paste your workflow (Ctrl + V or Cmd + V).
7. Click on the **_Publish Workflow to Share_** button to share your workflow.

<figure><img src="/_images/courses/level-one/chapter-three/share-workflow.png" alt="Share workflow" style="width:100%"><figcaption align = "center"><i>Share workflow</i></figcaption></figure>

Next, your workflow will be reviewed by our team. If it meets our guidelines, it will appear on the n8n workflows page for everyone to see and use!
-->
