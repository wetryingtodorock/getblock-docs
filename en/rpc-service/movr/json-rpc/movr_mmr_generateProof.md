---
title: movr:mmr_generateProof  {disallowed} - Moonriver
description: Example code for the movr:mmr_generateProof  {disallowed} json-rpc method. Сomplete guide on how to use movr:mmr_generateProof  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`leafIndex` - u64

leaf index.

`at` - BlockHash

Hash of the block.

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "mmr_generateProof",
"params": [null, null],
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

