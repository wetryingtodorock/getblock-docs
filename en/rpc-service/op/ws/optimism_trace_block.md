---
title: optimism:trace_block - Optimism
description: Example code for the optimism:trace_block ws method. Сomplete guide on how to use optimism:trace_block ws in GetBlock.io Web3 documentation.
---

### Parameters


`quantity|tag` - string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "trace_block",
"params": ["latest"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method trace_block does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

