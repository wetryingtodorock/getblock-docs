---
title: bsc:debug_standardTraceBlockToFile \[WebSocket\] {disallowed}
description: Generates files containing the block trace. A separate file is generatedfor each transaction in the block.You can also specify a trace file for a specific transaction in a block.Use debug_standardTraceBadBlockToFile to view the trace for an invalidblock.
---

### Parameters


`blockHash` - data

Block hash.

`txHash` - data

The transaction hash. Optional. If omitted, then a trace file is
generated for each transaction in the block.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_standardTraceBlockToFile",
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

