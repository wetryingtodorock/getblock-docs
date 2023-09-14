---
title: arbitrum:eth_newBlockFilter \[POST\]
description: Creates a filter in the node, to notify when a new block arrives. Tocheck if the state has changed, call eth_getFilterChanges.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://arbitrum.getblock.io/mainnet/' 
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
    "result": "0x6aacc1719383adeb356a720506fd2064"
}
```

