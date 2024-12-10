---
title: bsc:debug_getBadBlocks  {disallowed} - Binance Smart Chain
description: Example code for the bsc:debug_getBadBlocks  {disallowed} ws method. Сomplete guide on how to use bsc:debug_getBadBlocks  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_getBadBlocks",
"params": [],
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

