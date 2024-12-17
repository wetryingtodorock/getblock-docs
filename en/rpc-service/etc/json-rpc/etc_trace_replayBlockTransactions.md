---
title: etc:trace_replayBlockTransactions \[POST\]
description: Provides transaction processing tracing per block.
---

### Parameters


`blockNumber` - string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

`options` - list of string

list of tracing options; tracing options are trace, vmTrace, and
stateDiff. Specify any combination of the three options including none
of them.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "trace_replayBlockTransactions",
"params": ["latest", ["trace", "vmTrace", "vmTrace"]],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": []
}
```

