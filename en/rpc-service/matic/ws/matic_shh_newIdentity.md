---
title: matic:shh_newIdentity  {disallowed} - Polygon
description: Example code for the matic:shh_newIdentity  {disallowed} ws method. Сomplete guide on how to use matic:shh_newIdentity  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "shh_newIdentity",
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

