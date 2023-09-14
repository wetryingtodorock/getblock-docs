---
title: neo:gettransactionheight \[POST\]
description: Returns the transaction height with the specified transaction hash.
---

### Parameters


`txid` - string

Transaction id.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "gettransactionheight",
"params": ["0x2b64b0823f61a6be1a9b9fe2767a1e06b12a563a5f1d994b9adbc2387a907144"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": 7901849
}
```

