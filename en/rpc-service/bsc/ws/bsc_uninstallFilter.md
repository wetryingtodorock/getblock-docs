---
title: bsc:uninstallFilter  {disallowed} - Binance Smart Chain
description: Example code for the bsc:uninstallFilter  {disallowed} ws method. Сomplete guide on how to use bsc:uninstallFilter  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY` - None

The filter id

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "uninstallFilter",
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

