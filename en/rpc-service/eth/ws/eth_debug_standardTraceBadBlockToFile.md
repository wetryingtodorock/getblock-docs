---
title: eth:debug_standardTraceBadBlockToFile \[WebSocket\] {disallowed}
description: Generates files containing the block trace of invalid blocks. A separatefile is generated for each transaction in the block.Use debug_standardTraceBlockToFile to view the trace for a valid block.
---

### Parameters


`blockHash` - data

Block hash

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_standardTraceBadBlockToFile",
"params": ["0x2dfcd01e308905d7a46187745f5e07606e31682c8443a171bb47ce3d399b5049"],
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

