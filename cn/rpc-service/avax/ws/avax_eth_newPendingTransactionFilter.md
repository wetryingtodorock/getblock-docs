---
title: avax:eth_newPendingTransactionFilter \[WebSocket\]
description: Creates a filter in the node, to notify when new pending transactionsarrive. To check if the state has changed, call eth_getFilterChanges.
---

### Parameters


\-

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "0x9c285759ef99de8af868a93282b1e9dd"
}
```

