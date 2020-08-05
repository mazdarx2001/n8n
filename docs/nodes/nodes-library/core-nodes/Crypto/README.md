---
permalink: /nodes/n8n-nodes-base.crypto
---

# Crypto

The Crypto node is used to encrypt data in workflows.

While sending sensitive information over the internet, like a RESTful API for example, you can use the Crypto node to encrypt your data.

- Hash your data when you want to protect the integrity of the message by encoding it.
- Hmac your data when you want to protect the message by encoding and encrypting it with a shared key
- Sign your data when you want to protect the message with asymmetric keys

Here is a quick table to help you choose the correct cryptographic method:

```
Cryptographic primitive | Hash |    MAC    | Digital
Security Goal           |      |           | signature
------------------------+------+-----------+-------------
Integrity               |  Yes |    Yes    |   Yes
Authentication          |  No  |    Yes    |   Yes
Non-repudiation         |  No  |    No     |   Yes
------------------------+------+-----------+-------------
Kind of keys            | none | symmetric | asymmetric
                        |      |    keys   |    keys
```

## Node Reference

- Action
	- Hash a text in a specified format
	- Hmac a text in a specified format
	- Sign a string using a private key

You can configure further options for each action by selecting the type of encryption and encoding to be used, in the _Type_ and _Encoding_ fields respectively.

- Type
    - MD5
    - SHA256
    - SHA512

- Encoding
	- BASE64
	- HEX

## Example Usage

This workflow allows you to encrypt data using the Crypto node. You can also find the [workflow](https://n8n.io/workflows/574) on the website. This example usage workflow would use the following two nodes.
- [Start](../../core-nodes/Start/README.md)
- [Crypto]()


The final workflow should look like the following image.

![A workflow with the Crypto node](./workflow.png)

### 1. Start node

The start node exists by default when you create a new workflow.

### 2. Crypto node

1. Enter the data that you want to encrypt in the *Value* field.
2. Click on *Execute Node* to run the workflow.
