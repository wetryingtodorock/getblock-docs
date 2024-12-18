---
title: /api/v1/allowancev2 - Ontology
description: Example code for the /api/v1/allowancev2 rest method. Сomplete guide on how to use /api/v1/allowancev2 rest in GetBlock.io Web3 documentation.
---

### Parameters


`asset` - path

string

Asset contract hash

`from` - path

string

Source account address

`to` - path

string

Recipient account address

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/allowance2/ont/A9yD14Nj9j7xAB4dbGeiX9h8unkKHxuWwb/AA4WVfUB1ipHL8s3PRSYgeV1HhAU3KcKTq' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getallowance",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": "10",
    "Version": "1.0.0"
}
```

