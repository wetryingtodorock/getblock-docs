---
title: matic:eth_newPendingTransactionFilter \[WebSocket\]
description: Creates a filter in the node, to notify when new pending transactionsarrive. To check if the state has changed, call eth_getFilterChanges.
---

### Parameters


\-

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_newPendingTransactionFilter",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0xb6df4dd8d5aca49432acd450aea8a159"
}
```

