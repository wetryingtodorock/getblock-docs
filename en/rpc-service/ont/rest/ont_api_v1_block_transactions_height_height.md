---
title: ont:/api/v1/block/transactions/height/{height} \[GET\]
description: Fetch all transaction hashes for a block at a given height
---

### Parameters


`height` - path

integer

block height

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/block/transactions/height/16242872' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getblocktxsbyheight",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": {
        "Hash": "d68a50c85d2ebe3e9c7b1613af3d588c65a64c1fa3043e58d4c6b70b51f5490e",
        "Height": 16242872,
        "Transactions": [
            "fb8660eee2cd98a8683daf4e06e0180b470896d68f6b8a4e4dffb1f18f68ff49"
        ]
    },
    "Version": "1.0.0"
}
```

