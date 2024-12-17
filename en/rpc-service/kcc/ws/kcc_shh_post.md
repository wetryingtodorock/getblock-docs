---
title: shh_post  {disallowed} - KuCoin Community Chain
description: Example code for the shh_post  {disallowed} ws method. Сomplete guide on how to use shh_post  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`None` - None

None

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "shh_post",
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

