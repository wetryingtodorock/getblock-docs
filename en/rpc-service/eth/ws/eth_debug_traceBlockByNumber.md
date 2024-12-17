---
title: eth:debug_traceBlockByNumber  {disallowed} - Ethereum
description: Example code for the eth:debug_traceBlockByNumber  {disallowed} ws method. Сomplete guide on how to use eth:debug_traceBlockByNumber  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`quantity|tag` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

`Object` - Object

request options (all optional and default to false)

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
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

