---
title: ont:getblocktxsbyheight \[POST\]
description: Fetches transaction hashes of all the transactions in the block at agiven height.
---

### Parameters


`height` - integer

block height

### Request

``` java
curl --location --request POST 'https://ont.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getblocktxsbyheight",
"params": [16224151],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "desc": "SUCCESS",
    "error": 0,
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "Hash": "b4553dd4a5b3255aa78d20b2f2f0ec9d3a52d6ef2c99bfa23fd1f67001d9dd8b",
        "Height": 16224151,
        "Transactions": []
    }
}
```

