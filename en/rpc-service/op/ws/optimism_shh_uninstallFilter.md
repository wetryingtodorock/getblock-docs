---
title: optimism:shh_uninstallFilter  {disallowed} - Optimism
description: Example code for the optimism:shh_uninstallFilter  {disallowed} ws method. Сomplete guide on how to use optimism:shh_uninstallFilter  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`id` - string

the filter id.

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "shh_uninstallFilter",
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

