---
title: Data security with Doc²
description: A lising of the data security messures of Doc²
tags:
  - DOC²
  - Data security
---

# Data security


### Uploaded files
All of the uploaded files are stored in an object storage hosted by our Cloud Provider. Access is restricted and only possible if you pass the correct key and secret key.

### Database 
We run daily database backups that are then saved for seven days each.  
The communication between the database and the servers is run only via https.  
Stored passwords are encrypted in a way that, even with access to the database, cannot be read.


### Server Communication
All communication is done via https, every non https request is redirected to https.

