---
title: shh_addToGroup  {disallowed} - KuCoin Community Chain
description: Example code for the shh_addToGroup  {disallowed} ws method. Сomplete guide on how to use shh_addToGroup  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`address` - data

The identity address to add to a group

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "shh_addToGroup",
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

