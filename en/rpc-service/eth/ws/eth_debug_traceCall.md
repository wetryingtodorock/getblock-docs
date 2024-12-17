---
title: eth:debug_traceCall  {disallowed} - Ethereum
description: Example code for the eth:debug_traceCall  {disallowed} ws method. Сomplete guide on how to use eth:debug_traceCall  {disallowed} ws in GetBlock.io Web3 documentation.
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
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_traceCall",
"params": [{"to": "0xd46e8dd67c5d32be8058bb8eb970870f07244567"}, "finalized", {"tracer": "callTracer"}],
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

