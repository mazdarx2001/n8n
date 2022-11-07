---
title: "Group function to extract data from tables"
description: The group function is one of the most important feature to extract data form tables. Once a table has been extracted via DOC² and the columns have been mapped the obtained data can be grouped to get a structured result set of all extracted data.
date: "2022-02-24"
tags:
  - Tables
  - Table Extraction
  - DOC²
---

# Group function to extract data from tables

Once a table has been extracted via DOC² and the columns have been mapped ([Mapping of columns](/doc2/table-extraction/mapping-of-columns/)), the obtained data can be grouped to get a structured result set of all extracted data.

[Sign up for a 30 days free trail](https://app.polydocs.io){ .md-button .md-button--primary }

## What does this mean?

All documents, from order confirmations to invoices, can vary in complexity from company to company. For example, in documents, information may be presented in tables in some columns across multiple rows and in other columns across only one row.

For example, you can see the German invoice below, where the information in column "Bezeichnung" extends over several lines (positions).

![](/_images/doc2/image-30-1024x636.png){ loading=lazy }

At this point, another advantage of DOC² comes into play. It extracts the data in the first step. The result looks like this:

![](/_images/doc2/image-31-1024x633.png){ loading=lazy }

BUT: It is now possible to group data based on a specific column. That means that, in this case, it can be grouped by the column "Position" as shown in the following video. This in turn groups the rows of the "Description" column into one row. So that at the end you get a structured overall picture of the export and the data can now be processed further.

If the grouping was created by mistake, it can be removed at any time, as also shown in the video.

The result of grouping looks like this:

![](/_images/doc2/image-32-1024x567.png){ loading=lazy }
