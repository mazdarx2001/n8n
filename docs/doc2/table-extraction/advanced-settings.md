---
title: "Advanced settings for table extraction"
description: In DOC² there are various advanced settings to extract a table. On this page you will find a few examples of different table characteristics.
date: "2022-03-01"
tags:
  - Table
  - DOC²
  - Settings
---

In table extraction view, you will find the menu item `Settings` in the upper action bar (make sure that "Training Mode" is activated). If you click on the gear icon, a window will open in which you will find `Advanced Settings`.

![](/_images/doc2/advanced-settings_1.png){ loading=lazy }



![](/_images/doc2/advanced-settings_2.png){ loading=lazy }

## These functionalities are available in "Settings":

#### Header row count

Here you can define the number of lines of a table header. For example, the table header line can be two lines:

![](/_images/doc2/advanced-settings_3.png){ loading=lazy }

Accordingly, the value in "Header row count" is set to two:

![](/_images/doc2/advanced-settings_4.png){ loading=lazy }

Why is this needed? It might be that DOC² does not recognize the second line in the table header as header line. In this case, it incorrectly inserts it into the table as an extracted value. This can easily be prevented with this function.

<ins>Example before</ins>:

![](/_images/doc2/advanced-settings_5.png){ loading=lazy }

<ins>Example after</ins>:

![](/_images/doc2/advanced-settings_6.png){ loading=lazy }


#### Move Extra Rows to

In this example, the item description in the table spans several rows, but you only need the first one. To only extract this and include it in the "DESCRIPTION" column, select `Move Extra Rows to` `Trash`.

![](/_images/doc2/advanced-settings_11.png){ loading=lazy }
![](/_images/doc2/advanced-settings_12.png){ loading=lazy }

 After naming the columns and mapping them to a position, you get the following result:

![](/_images/doc2/advanced-settings_13.png){ loading=lazy }



## Below functionalities are available in the advanced settings:

![](/_images/doc2/advanced-settings_15.png){ loading=lazy }


#### Minimum grouped rows

Enter the minimum number of rows in your grouped column here.

![](/_images/doc2/advanced-settings_16.png){ loading=lazy }

In this table you see six rows of which only three would be relevant to you. In the first two columns there are two criteria that have to be extracted separately. These will be your mapped columns, all the other ones have to be trained as custom columns. <br> It works as follows:

Select the two [header rows](/doc2/table-extraction/advanced-settings/#header-row-count) as well as two minimum grouped rows as these should be grouped to one row.

![](/_images/doc2/advanced-settings_17.png){ loading=lazy }
![](/_images/doc2/advanced-settings_18.png){ loading=lazy }

Also select the `Move extra rows to` `Trash` option to be able to train all the other columns as custom columns.

![](/_images/doc2/advanced-settings_19.png){ loading=lazy }

Name the first column "Position" and group on that one.

![](/_images/doc2/advanced-settings_20.png){ loading=lazy }

After naming all the columns and training the values, this should be your result:


![](/_images/doc2/advanced-settings_21.png){ loading=lazy }



<!--

##### Maximum grouped rows

Enter the maximum number of rows in your grouped column here.

#### Distinct group columns

If you want only unique values for your grouped column, check the box here.

-->

#### Reverse grouping

If you want to combine all the rows above the grouped attribute, check the box here.

In this example, the table starts with a row that is above all other information but also needs to be extracted along with the information below it. DOC² might extract this row as an additional row and then the grouping of the information, e.g. by position, will not work properly.

![](/_images/doc2/advanced-settings_7.png){ loading=lazy }
![](/_images/doc2/advanced-settings_9.png){ loading=lazy }

After grouping on net amount, checking the box, selecting the `Move extra rows to` `Trash` option 

![](/_images/doc2/advanced-settings_9.1.png){ loading=lazy }

and naming all columns this is your result:

![](/_images/doc2/advanced-settings_10.png){ loading=lazy }
<!--

#### Split Text

If you want to split the text exactly at the column separator, check the box here. -->