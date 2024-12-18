---
title: compileSerpent  {disallowed} - Binance Smart Chain
description: Example code for the compileSerpent  {disallowed} ws method. Сomplete guide on how to use compileSerpent  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`String` - hex string

The source code.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "compileSerpent",
"params": [null],
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

