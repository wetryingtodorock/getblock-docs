---
title: rsk:eth_newBlockFilter \[POST\]
description: Creates a filter in the node, to notify when a new block arrives. Tocheck if the state has changed, call eth_getFilterChanges.
---

### Parameters


\-

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_newBlockFilter",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x5e90"
}
```

