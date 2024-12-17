---
title: bsc:trace_block - Binance Smart Chain
description: Example code for the bsc:trace_block ws method. Сomplete guide on how to use bsc:trace_block ws in GetBlock.io Web3 documentation.
---

### Parameters


`quantity|tag` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "trace_block",
"params": ["0x6"],
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

