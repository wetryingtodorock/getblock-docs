---
title: bsc:debug_standardTraceBadBlockToFile \[WebSocket\] {disallowed}
description: Generates files containing the block trace of invalid blocks. A separatefile is generated for each transaction in the block.Use debug_standardTraceBlockToFile to view the trace for a valid block.
---

### Parameters


`blockHash` - data

Block hash

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_standardTraceBadBlockToFile",
"params": ["0x0cf46846c9f2abef8e40ed2f8deea4b789464f44284efe25d443e8d272393fce"],
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

