---
title: kcc:shh_newIdentity  {disallowed} - KuCoin Community Chain
description: Example code for the kcc:shh_newIdentity  {disallowed} ws method. Сomplete guide on how to use kcc:shh_newIdentity  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
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

