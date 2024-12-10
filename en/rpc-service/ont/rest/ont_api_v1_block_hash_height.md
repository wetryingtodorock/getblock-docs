---
title: ont:/api/v1/block/hash/{height} - Ontology
description: Example code for the ont:/api/v1/block/hash/{height} rest method. Сomplete guide on how to use ont:/api/v1/block/hash/{height} rest in GetBlock.io Web3 documentation.
---

### Parameters


`height` - path

integer

block height

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/block/hash/16242872' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getblockhash",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": "d68a50c85d2ebe3e9c7b1613af3d588c65a64c1fa3043e58d4c6b70b51f5490e",
    "Version": "1.0.0"
}
```

