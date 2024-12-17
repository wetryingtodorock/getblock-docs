---
title: /api/v1/mempool/txstate/{hash} - Ontology
description: Example code for the /api/v1/mempool/txstate/{hash} rest method. Сomplete guide on how to use /api/v1/mempool/txstate/{hash} rest in GetBlock.io Web3 documentation.
---

### Parameters


`hash` - path

string

Tranaction hash

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest//api/v1/mempool/txstate/db81c4e00f050c4f8e2f9c7e8201fddebd18458b3c48c73c18aa0532c7b5c43c' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getmempooltxstate",
    "Desc": "SUCCESS",
    "Error": 0,
    "Version": "1.0.0",
    "Result": {
        "State": [
            {
                "Type": 1,
                "Height": 342,
                "ErrCode": 0
            },
            {
                "Type": 0,
                "Height": 0,
                "ErrCode": 0
            }
        ]
    }
}
```

