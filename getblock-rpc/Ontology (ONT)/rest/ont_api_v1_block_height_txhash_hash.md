---
title: /api/v1/block/height/txhash/{hash} - Ontology
description: Example code for the /api/v1/block/height/txhash/{hash} rest method. Сomplete guide on how to use /api/v1/block/height/txhash/{hash} rest in GetBlock.io Web3 documentation.
---

### Parameters


`hash` - path

Tranaction hash

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/block/height/txhash/db81c4e00f050c4f8e2f9c7e8201fddebd18458b3c48c73c18aa0532c7b5c43c' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getblockheightbytxhash",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": 16224161,
    "Version": "1.0.0"
}
```

