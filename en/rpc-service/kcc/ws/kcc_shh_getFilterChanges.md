---
title: kcc:shh_getFilterChanges  {disallowed} - KuCoin Community Chain
description: Example code for the kcc:shh_getFilterChanges  {disallowed} ws method. Сomplete guide on how to use kcc:shh_getFilterChanges  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`id` - string

the filter id.

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "shh_getFilterChanges",
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

