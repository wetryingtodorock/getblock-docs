---
title: bsc:debug_standardTraceBlockToFile  {disallowed} - Binance Smart Chain
description: Example code for the bsc:debug_standardTraceBlockToFile  {disallowed} json-rpc method. Сomplete guide on how to use bsc:debug_standardTraceBlockToFile  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`blockHash` - data

Block hash.

`txHash` - data

The transaction hash. Optional. If omitted, then a trace file is
generated for each transaction in the block.

### Request

``` java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "debug_standardTraceBlockToFile",
"params": ["0x0cf46846c9f2abef8e40ed2f8deea4b789464f44284efe25d443e8d272393fce", null],
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

