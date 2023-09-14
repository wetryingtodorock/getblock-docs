---
title: eth:debug_traceCall \[POST\] {disallowed}
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
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "debug_traceCall",
"params": [{"to": "0xd46e8dd67c5d32be8058bb8eb970870f07244567"}, "finalized", {"tracer": "callTracer"}],
"id": "getblock.io"}'
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

