---
title: debug_standardTraceBlockToFile  {disallowed} - Ethereum
description: Example code for the debug_standardTraceBlockToFile  {disallowed} json-rpc method. Сomplete guide on how to use debug_standardTraceBlockToFile  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`blockHash` - data

Block hash.

`txHash` - data

The transaction hash. Optional. If omitted, then a trace file is
generated for each transaction in the block.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "debug_standardTraceBlockToFile",
"params": ["0x2dfcd01e308905d7a46187745f5e07606e31682c8443a171bb47ce3d399b5049", null],
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

