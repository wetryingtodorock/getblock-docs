---
title: dash:/mempool/contents.json - Dash
description: Example code for the dash:/mempool/contents.json rest method. Сomplete guide on how to use dash:/mempool/contents.json rest in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://dash.getblock.io/mainnet/mempool/contents.json' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "046440a5ae8a6a69da5895f5edecbe7ba4558f40f7396526812b261ef3fee824": {
        "ancestorcount": 1,
        "ancestorfees": 374,
        "ancestorsize": 338,
        "depends": [],
        "descendantcount": 1,
        "descendantfees": 374,
        "descendantsize": 338,
        "fee": 3.74e-06,
        "fees": {
            "ancestor": 3.74e-06,
            "base": 3.74e-06,
            "descendant": 3.74e-06,
            "modified": 3.74e-06
        },
        "height": 1891101,
        "instantlock": "true",
        "modifiedfee": 3.74e-06,
        "spentby": [],
        "time": 1687340315,
        "vsize": 338
    }
}
```

