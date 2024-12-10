---
title: optimism:eth_getFilterLogs - Optimism
description: Example code for the optimism:eth_getFilterLogs ws method. Сomplete guide on how to use optimism:eth_getFilterLogs ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY` - string

The filter id.

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getFilterLogs",
"params": ["0x16"],
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

