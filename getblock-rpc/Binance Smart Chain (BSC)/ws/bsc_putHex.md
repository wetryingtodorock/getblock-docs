---
title: putHex  {disallowed} - Binance Smart Chain
description: Example code for the putHex  {disallowed} ws method. Сomplete guide on how to use putHex  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`String` - None

Database name

`String` - None

Key name

`DATA` - None

The data to store

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "putHex",
"params": [null, null, null],
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

