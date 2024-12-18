---
title: debug_storageRangeAt  {disallowed} - Binance Smart Chain
description: Example code for the debug_storageRangeAt  {disallowed} ws method. Сomplete guide on how to use debug_storageRangeAt  {disallowed} ws in GetBlock.io Web3 documentation.
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
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_storageRangeAt",
"params": ["0x6e6a058ac35224a9842a8010042ddc93dea2f073260a8d79cd3368a232c3e7ed", 3, "0x0a8156e7ee392d885d10eaa86afd0e323afdcd95", "0xc94770007dda54cF92009BFF0dE90c06F603a09f", 1],
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

