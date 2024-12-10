---
title: bsc:debug_traceTransaction  {disallowed} - Binance Smart Chain
description: Example code for the bsc:debug_traceTransaction  {disallowed} ws method. Сomplete guide on how to use bsc:debug_traceTransaction  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`transactionHash` - data

Transaction hash.

`Object` - None

request options (all optional and default to false)

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_traceTransaction",
"params": ["0xcd718a69d478340dc28fdf6bf8056374a52dc95841b44083163ced8dfe29310c", null],
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

