---
title: bsc:debug_traceBlockByHash \[WebSocket\] {disallowed}
description: Returns full trace of all invoked opcodes of all transactions includedin the block.
---

### Parameters


`block hash` - data

Block hash.

`Object` - None

request options (all optional and default to false)

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_traceBlockByHash",
"params": ["0x0cf46846c9f2abef8e40ed2f8deea4b789464f44284efe25d443e8d272393fce", null],
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

