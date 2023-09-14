---
title: bsc:trace_replayBlockTransactions \[WebSocket\]
description: Provides transaction processing tracing per block.
---

### Parameters


`quantity|tag` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

`array of strings` - None

Tracing options are trace, vmTrace, and stateDiff. Specify any
combination of the three options including none of them.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "trace_replayBlockTransactions",
"params": ["0x12", ["trace", "vmTrace", "vmTrace"]],
"id": "getblock.io"}
```

###  Response

``` java
{
    "error": {
        "code": -32601,
        "message": "the method trace_replayBlockTransactions does not exist/is not available"
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

