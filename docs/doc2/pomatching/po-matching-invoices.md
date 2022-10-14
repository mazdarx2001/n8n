---
title: "PO Matching - Invoices"
description: Step by step guide how to create a purchase order in LN, Upload the invoice in DOC², handle two different scenarios and check the receipt of the invoice in LN.
date: "2022-01-24"
tags:
  - DOC²
  - PO Matching
  - Invoice
  - LN
---

# PO Matching - Invoices

## Create a purchase order in LN

Open LN and go to Purchase Order Intake Workbench


![](/_images/doc2/LN_PO-Intake-Workbench.png)

Select Purchase Orders

![](/_images/doc2/LN_Purchase-Orders-1-1024x263.png)

and add a new one by choosing the + symbol

![](/_images/doc2/LN_PO_new-1024x149.png)

Now you can create the document and the corresponding table and its values.

First add the Business Partner via the search function (the magnifying glas), clicking out of the marked field, fills the rest of them with the stored data.

![](/_images/doc2/LN_PO_Business-Partner-1024x402.png)

For the next step add the order lines. You need to add each line manually and need to input the Item and order Quantity – the rest will be filled automatically.

![](/_images/doc2/LN_PO_Order-Lines-1-1024x147.png)

After that save the purchase order. You must **approve** said purchase order and so that the settings are relayed to the system.

![](/_images/doc2/LN_PO_Approve-1024x528.png)

* * *

[Sign up for a 30 days free trail](https://app.polydocs.io){ .md-button .md-button--primary }

## Upload the Invoice in DOC2

![](/_images/doc2/DOC2_POM_Invoices_1.png)

The symbol under **MATCHED** indicates the current matching status – green for matched and red for not matched. Ideally it is already green.

Open the document and validate the extracted fields.

![](/_images/doc2/DOC2_POM_Invoices_2.png)

* * *

After validating all extracted fields open matching overview by clicking on **PO MATCHING**

![](/_images/doc2/DOC2_POM_Invoices_3.png)

You can also go directly from dashboard to the matching overview by following the steps [below](/doc2/pomatching/po-matching-invoices/#case-1-matched)

* * *

The symbol under **MATCHED** indicates the current matching status – green for matched and red for not matched. Ideally it is already green.

![](/_images/doc2/DOC2_POM_Invoices_4.png)

### Case 1: Matched

Access the matching overview by clicking on the Matching Symbol on the dashboard.

![](/_images/doc2/DOC2_POM_Invoices_5.png)

![](/_images/doc2/DOC2_POM_Invoices_6.png)

In this case the quantity of items ordered matches the quantity on the invoice, the match and thus the document can be validated and exported.

![](/_images/doc2/DOC2_POM_Invoices_7.png)

invoice exporting

![](/_images/doc2/DOC2_POM_Invoices_8.png)

exported successfully

* * *

### Case 2: Not matched

Access the matching overview by clicking on the Matching Symbol on the dashboard.

![](/_images/doc2/DOC2_POM_Invoices_9.png)

![](/_images/doc2/DOC2_POM_Invoices_10.png)

Here you can see that the quantity of the ordered item does not match the quantity on the invoice.

The matches can now be corrected:

The “x” would delete the match on the invoice.

A new match from the purchase order can be added to the invoice by dragging and dropping the appropriate data row(s).

![](/_images/doc2/DOC2_POM_Invoices_11.png)

You need to confirm the mismatched properties.

![](/_images/doc2/DOC2_POM_Invoices_12.png)

![](/_images/doc2/DOC2_POM_Invoices_13.png)

Save to apply all changes.

![](/_images/doc2/DOC2_POM_Invoices_14.png)

Once everything is correct the document can be validated and exported.

![](/_images/doc2/DOC2_POM_Invoices_7.png)

invoice exporting

![](/_images/doc2/DOC2_POM_Invoices_8.png)

exported successfully

![This image has an empty alt attribute; its file name is Attention-Warning.png](/_images/doc2/Attention-Warning.png)

Since in LN no comparison regarding the quantity between order and invoice is possible, in this case you have to make the comparison with the delivery bill. You can find out how this works [here](/doc2/pomatching/po-matching-delivery-notes/).

* * *

## Check the receipt of the invoice in LN

To see if the process was successful, you can check this in LN by choosing “Process Payables Workbench”

![](/_images/doc2/LN_Process-Payables-Workbench-702x1024.png)

![](/_images/doc2/LN_Search-invoice-no-1-1024x118.png)

Search by invoice number in the corresponding field

![](/_images/doc2/LN_Icon-to-open-overview-1024x119.png)

If you click on this icon, the following overview will open, in which you will see the order and the assigned invoice.

![](/_images/doc2/LN_Matched-Invoice-1024x551.png)
