---
title: zec:getmempoolinfo - Zcash
description: Example code for the zec:getmempoolinfo json-rpc method. Сomplete guide on how to use zec:getmempoolinfo json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getmempoolinfo",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "bytes": 22506,
        "size": 18,
        "usage": 54000
    }
}
```

