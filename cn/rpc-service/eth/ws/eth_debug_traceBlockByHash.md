---
title: eth:debug_traceBlockByHash \[WebSocket\] {disallowed}
description: Returns full trace of all invoked opcodes of all transactions includedin the block.
---

### Parameters


`block hash` - data

Block hash.

`Object` - None

request options (all optional and default to false)

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_traceBlockByHash",
"params": ["0x2dfcd01e308905d7a46187745f5e07606e31682c8443a171bb47ce3d399b5049", null],
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

