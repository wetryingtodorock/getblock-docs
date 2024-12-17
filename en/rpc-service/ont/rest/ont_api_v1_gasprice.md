---
title: ont:/api/v1/gasprice \[GET\]
description: Fetch gas price for transaction
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

