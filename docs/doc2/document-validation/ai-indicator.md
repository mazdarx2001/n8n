---
title: "AI Indicators"
description: In the documentation you will find options to display the quality of the extraction using graphical indicators. The so-called AI indicator.
date: "2022-03-23"
tags:
  - AI
  - DOC²
---

In document view you will find options to display the quality of the extraction using graphical indicators. The so-called AI indicator.

To do this, open a document as known via the dashboard:

![](/_images/doc2/image-50-1024x391.png)

In document view there are two indicators for the quality of the extraction.

- Extraction quality in percent per field and current document
- Overall extraction quality including previous extractions of documents of the same type.

![](/_images/doc2/image-51-1024x474.png){ loading=lazy }

**Extraction quality in percent per field and current document**

For each field there is a value available on the right side which indicates the quality of extraction for the current document. A percentage value will be displayed:

![](/_images/doc2/image-52.png){ loading=lazy }

**Overall extraction quality including previous extractions of documents of the same type**

Furthermore, there is a graph that shows the quality of all previous extractions for a document type. This refers in each case to the extraction value with the lowest quality:

![](/_images/doc2/image-53.png){ loading=lazy }

**Technical Details:**

The AI indicator shows how well a document is trained. This is done via an internal score. This means that as soon as a document is read in and the fields extracted by DOC² are confirmed by the user, this score is increased. The higher the score, the further the display of the AI indicator will be in the green area. If fields are changed manually by the user after the export, this score will decrease again and the display of the AI indicator will fall back into the red area. Only when the document has been taught and the extraction has determined the correct value for some imports without manual intervention will the score reach 100%.
