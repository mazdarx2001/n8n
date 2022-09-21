---
title: DOC² to Infor OS
description: Documentation for Export DOC² to Infor OS
tags:
  - DOC²
  - Export
  - Infor
  - DOC²
---

# Export to Infor :fontawesome-solid-file-export:



``` mermaid
graph LR
  A[Start] --> B{Invoice?};
  B -->|Yes| C[Extraction];
  C --> D[Infor LN or M3];
  D --> E[Send to IDM];
  B ---->|No| E[Send to IDM];
  E --> F[End];
```



Here you can find all the useful pages to connect your infor environment correctly:

- [:octicons-file-24: How to create a BOD mapping file](/doc2/export/how-to-create-a-bod-mapping-file/)
- [:fontawesome-solid-file-export: Export to Infor ION and IDM](/doc2/export/infor-ion/)
- [:octicons-file-24: How to create a IDM mapping file](/doc2/export/how-to-create-a-idm-mapping-file/)
- [:octicons-file-24: How to create an Infor ION API file](/doc2/export/create-a-infor-ion-api-file/)
- [:fontawesome-solid-file-export: Export to Infor IDM](/doc2/export/infor-idm/)
