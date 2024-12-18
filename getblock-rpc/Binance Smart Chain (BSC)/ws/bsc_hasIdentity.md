---
title: hasIdentity  {disallowed} - Binance Smart Chain
description: Example code for the hasIdentity  {disallowed} ws method. Сomplete guide on how to use hasIdentity  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - None

60 Bytes - The identity address to check.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "hasIdentity",
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

