---
title: /api/v1/gasprice - Ontology
description: Example code for the /api/v1/gasprice rest method. Сomplete guide on how to use /api/v1/gasprice rest in GetBlock.io Web3 documentation.
---

### Parameters


`hash` - path

Tranaction hash

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/gasprice' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getgasprice",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": {
        "gasprice": 2500,
        "height": 16248538
    },
    "Version": "1.0.0"
}
```

