---
title: List view
description: 
tags:
  - Insight²
  - Widgets
---

# List view

List view widget allows to create a list of repeatable rows of data. Just like container widget, you can nest other widgets inside of it and control how many times they repeat.



![Insight² - List view widget](/_images/insight2/widgets/list-view/listviewapp.png)



## Event

### Row clicked



![Insight² - List view widget](/_images/insight2/widgets/list-view/event.png)



To add an event to a button, click on the widget handle to open the widget properties on the right sidebar. Go to the **Events** section and click on **Add handler**.

**Row clicked** event is triggered when the button is clicked. Just like any other event on Insight, you can set multiple handlers for row clicked event.


Check [Action Reference](/insight2/actions/actions/) docs to get the detailed information about all the **Actions**.


## Properties



![Insight² - List view widget](/_images/insight2/widgets/list-view/properties.png)



| Properties  | description | Expected value |
| ----------- | ----------- | -------------- |
| List data | Enter the data that you want to diplay into the widget. Data in the form of array of objects or data from a query that returns an array of objects.| `{{ [ {id: 0, name: ABC, email: abc@bla.com}, {id: 1, name: XYZ, email: xyz@bla.com} ] }}` or `{{queries.xyz.data}}` |
| Row height | Enter a numerical value to set the row height accordingly. | Any number between `1` to `100` |
| Show bottom border | This property allows you to show or hide the row botton border. | By deafult its `{{true}}`, set `{{false}}` to hide the border  |

## Layout



![Insight² - List view widget](/_images/insight2/widgets/list-view/listlayout.png)


| Layout  | description | Expected value |
| ----------- | ----------- | ------------ |
| Show on desktop | Toggle on or off to display desktop view. | You can programmatically determing the value by clicking on `Fx` to set the value `{{true}}` or `{{false}}` |
| Show on mobile | Toggle on or off to display mobile view. | You can programmatically determing the value by clicking on `Fx` to set the value `{{true}}` or `{{false}}`   |

## Styles



![Insight² - List view widget](/_images/insight2/widgets/list-view/style.png)



| Style      | Description |
| ----------- | ----------- |
| backgroundColor |  You can change the background color of the widget by entering the Hex color code or choosing a color of your choice from the color picker. |
| Visibility | This is to control the visibility of the widget. If `{{false}}` the widget will not visible after the app is deployed. It can only have boolean values i.e. either `{{true}}` or `{{false}}`. By default, it's set to `{{true}}`. |
| Disable |  This property only accepts boolean values. If set to `{{true}}`, the widget will be locked and becomes non-functional. By default, its value is set to `{{false}}`. |


Any property having `Fx` button next to its field can be **programmatically configured**.


## Example: Displaying data in the list view

- Let's start by creating a new app and then dragging the List view widget onto the canvas.



![Insight² - List view widget](/_images/insight2/widgets/list-view/emptylist_in2.png)



- Now lets create a query and select REST API from the datasource dropdown. Chose the `GET` method and enter the API endpoint - `https://reqres.in/api/users?page=1`. Save this query and fire it. Inspect the query results from the left sidebar, you'll see that it resulted the `data` object having array of objects.



![Insight² - List view widget](/_images/insight2/widgets/list-view/data.gif)


- Now lets edit the `List data` property of list view widget for displaying the query data. We will use JS to get the data from the query - `{{queries.restapi1.data.data}}`. Here the last `data` is data object that includes array of objects, the first `data` is the data resulted from the `restapi1` query. This will automatically create the rows in the widget using the data.



![Insight² - List view widget](/_images/insight2/widgets/list-view/datadisplay_in2.png)



- Finally, we will need to nest widgets into the first row of list view widget and the widget will automatically create the subsequent instances. The subsequent rows will appear the same way you'll display the data in the first row.



![Insight² - List view widget](/_images/insight2/widgets/list-view/addingwidgets_in2.gif)




Use `{{listItem.key}}` to display data on the nested widgets. Example: For displaying the images we used `{{listItem.avatar}}` where **avatar** is one of the key in the objects from the query result.


