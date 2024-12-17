---
title: eth_getFilterChanges - Gnosis
description: Example code for the eth_getFilterChanges ws method. Сomplete guide on how to use eth_getFilterChanges ws in GetBlock.io Web3 documentation.
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

