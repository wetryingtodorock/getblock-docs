---
title: arbitrum:shh_newGroup  {disallowed} - Arbitrum
description: Example code for the arbitrum:shh_newGroup  {disallowed} ws method. Сomplete guide on how to use arbitrum:shh_newGroup  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://arbitrum.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "shh_newGroup",
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

