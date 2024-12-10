---
title: etc:debug_standardTraceBlockToFile  {disallowed} - Ethereum Classic
description: Example code for the etc:debug_standardTraceBlockToFile  {disallowed} json-rpc method. Сomplete guide on how to use etc:debug_standardTraceBlockToFile  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`blockHash` - data

Block hash.

`txHash` - data

The transaction hash. Optional. If omitted, then a trace file is
generated for each transaction in the block.

`disableMemory` - boolean

Specify whether to capture EVM memory during the trace. Defaults to
true.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "debug_standardTraceBlockToFile",
"params": [null, null, false],
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

