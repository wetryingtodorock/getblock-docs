---
title: gno:eth_getFilterChanges \[WebSocket\]
description: Polls the specified filter and returns an array of changes that haveoccurred since the last poll.
---

### Parameters


`data` - hex string

Filter ID.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getFilterChanges",
"params": ["0x7c31"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "Filter not found"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

