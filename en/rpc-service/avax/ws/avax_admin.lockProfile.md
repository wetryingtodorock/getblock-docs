---
title: avax:admin.lockProfile  {disallowed} - Avalanche
description: Example code for the avax:admin.lockProfile  {disallowed} ws method. Сomplete guide on how to use avax:admin.lockProfile  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "admin.lockProfile",
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

