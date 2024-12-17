---
title: eth_getAssetBalance  {disallowed} - Avalanche
description: Example code for the eth_getAssetBalance  {disallowed} ws method. Сomplete guide on how to use eth_getAssetBalance  {disallowed} ws in GetBlock.io Web3 documentation.
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
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getAssetBalance",
"params": ["0x8723e5773847A4Eb5FeEDabD9320802c5c812F46", "latest", "3RvKBAmQnfYionFXMfW5P8TDZgZiogKbHjM8cjpu16LKAgF5T"],
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

