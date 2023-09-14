---
title: bsc:debug_traceCall \[WebSocket\]
description: Returns a transaction trace object.
---

### Parameters


`Object` - None

The transaction call object.

`DATA` - None

The block number in hex format, tags or the block hash.

`DATA` - None

The type of tracer.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_traceCall",
"params": [{"to": "0xd46e8dd67c5d32be8058bb8eb970870f07244567"}, "finalized", {"tracer": "callTracer"}],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "from": "0x0000000000000000000000000000000000000000",
        "gas": "0x17d2638",
        "gasUsed": "0x5208",
        "input": "0x",
        "to": "0xd46e8dd67c5d32be8058bb8eb970870f07244567",
        "type": "CALL",
        "value": "0x0"
    }
}
```

