---
title: ftm:eth_newBlockFilter \[POST\]
description: Creates a filter in the node, to notify when a new block arrives. Tocheck if the state has changed, call eth_getFilterChanges.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ftm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_newBlockFilter",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x91ade735d8e534290b7f774fd0e00b40"
}
```

