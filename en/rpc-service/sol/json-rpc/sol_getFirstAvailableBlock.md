---
title: sol:getFirstAvailableBlock \[POST\]
description: Returns the slot of the lowest confirmed block that has not been purgedfrom the ledger
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getFirstAvailableBlock",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": 122257143
}
```

