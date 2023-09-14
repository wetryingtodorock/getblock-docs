---
title: bsc:debug_traceBlockByNumber \[WebSocket\] {disallowed}
description: Returns full trace of all invoked opcodes of all transactions includedin the block.
---

### Parameters


`quantity|tag` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

`Object` - object

request options (all optional and default to false)

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_traceBlockByNumber",
"params": ["0xA1", {"tracer": "callTracer"}],
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

