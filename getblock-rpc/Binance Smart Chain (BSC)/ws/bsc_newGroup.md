---
title: newGroup  {disallowed} - Binance Smart Chain
description: Example code for the newGroup  {disallowed} ws method. Сomplete guide on how to use newGroup  {disallowed} ws in GetBlock.io Web3 documentation.

### Parameters


\-

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "newGroup",
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

