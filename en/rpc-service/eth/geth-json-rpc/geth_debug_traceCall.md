---
title: geth:debug_traceCall \[POST\] {disallowed}
description: The debug_traceCall method lets you run an eth_call within the contextof the given block execution using the final state of parent block asthe base. The first argument (just as in eth_call) is a transactionobject. The block can be specified either by hash or by number as thesecond argument. A tracer can be specified as a third argument, similarto debug_traceTransaction. It returns the same output asdebug_traceTransaction.
---

### Parameters


`object` - json object

call object

`blockNrOrHash` - string

number of a hash of a block

`options` - array of string

additional options

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_traceCall",
"params": [null, null, null],
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

