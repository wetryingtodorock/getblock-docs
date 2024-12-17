---
title: avax:eth_getAssetBalance \[POST\] {disallowed}
description: In addition to the standard Ethereum APIs, Avalanche offerseth_getAssetBalance to retrieve the balance of first class AvalancheNative Tokens on the C-Chain (excluding AVAX, which must be fetched witheth_getBalance).
---

### Parameters


`address` - string

owner of the asset

`blk` - blkNrOrHash

blk is the block number or hash at which to retrieve the balance

`assetID` - string

id of the asset for which the balance is requested

### Request

``` java
curl --location --request POST 'https://avax.getblock.io/mainnet/ext/bc/C/rpc' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getAssetBalance",
"params": ["0x8723e5773847A4Eb5FeEDabD9320802c5c812F46", "latest", "3RvKBAmQnfYionFXMfW5P8TDZgZiogKbHjM8cjpu16LKAgF5T"],
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

