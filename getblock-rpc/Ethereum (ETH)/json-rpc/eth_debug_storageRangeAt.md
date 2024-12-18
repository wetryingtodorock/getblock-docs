---
title: debug_storageRangeAt  {disallowed} - Ethereum
description: Example code for the debug_storageRangeAt  {disallowed} json-rpc method. Сomplete guide on how to use debug_storageRangeAt  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`blockHash` - data

Block hash.

`txIndex` - integer

Transaction index from which to start.

`address` - data

Contract address.

`startKey` - hash

Start key.

`limit` - integer

Number of storage entries to return.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "debug_storageRangeAt",
"params": ["0x340e1e44e8f6e6b0cd8d255d4fdaec2987bb073f02c62e068ed75d80f9890d5f", 3, "0x0a8156e7ee392d885d10eaa86afd0e323afdcd95", "0xc94770007dda54cF92009BFF0dE90c06F603a09f", 1],
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

