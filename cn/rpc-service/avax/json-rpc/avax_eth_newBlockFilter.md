---
title: avax:eth_newBlockFilter \[POST\]
description: Creates a filter in the node, to notify when a new block arrives. Tocheck if the state has changed, call eth_getFilterChanges.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
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
    "result": "0xde660a80c2931ac342ec8c086baa2f09"
}
```

