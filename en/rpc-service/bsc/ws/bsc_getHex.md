---
title: bsc:getHex  {disallowed} - Binance Smart Chain
description: Example code for the bsc:getHex  {disallowed} ws method. Сomplete guide on how to use bsc:getHex  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`String` - None

Database name

`String` - None

Key name

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "getHex",
"params": [null, null],
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

