---
title: heco:eth_getFilterChanges - Huobi ECO Chain
description: Example code for the heco:eth_getFilterChanges ws method. Сomplete guide on how to use heco:eth_getFilterChanges ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY` - string

The filter id.

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getFilterChanges",
"params": ["0x7373bf81a29e9491199289fab72c499f"],
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

