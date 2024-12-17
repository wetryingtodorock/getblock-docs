---
title: debug_standardTraceBadBlockToFile  {disallowed} - Binance Smart Chain
description: Example code for the debug_standardTraceBadBlockToFile  {disallowed} ws method. Сomplete guide on how to use debug_standardTraceBadBlockToFile  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`blockHash` - data

Block hash

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_standardTraceBadBlockToFile",
"params": ["0x0cf46846c9f2abef8e40ed2f8deea4b789464f44284efe25d443e8d272393fce"],
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

