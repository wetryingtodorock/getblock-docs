---
title: dot:mmr_verifyProof  {disallowed} - Polkadot
description: Example code for the dot:mmr_verifyProof  {disallowed} json-rpc method. Сomplete guide on how to use dot:mmr_verifyProof  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`proof` - MmmLeafBatchProof

mmr leaf batch proof

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "mmr_verifyProof",
"params": [null],
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

