---
title: eth:trace_replayBlockTransactions \[WebSocket\] {disallowed}
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
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "trace_replayBlockTransactions",
"params": ["0x12", ["trace", "vmTrace", "vmTrace"]],
"id": "getblock.io"}
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

