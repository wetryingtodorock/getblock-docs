---
title: bsc:eth_getFilterChanges - Binance Smart Chain
description: Example code for the bsc:eth_getFilterChanges ws method. Сomplete guide on how to use bsc:eth_getFilterChanges ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - hex string

Filter ID.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getFilterChanges",
"params": ["0x7c3173bd21b6fd2ad8be24c9aa40e8d9"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32000,
        "message": "filter not found"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

