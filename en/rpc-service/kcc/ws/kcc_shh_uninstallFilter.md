---
title: kcc:shh_uninstallFilter \[WebSocket\] {disallowed}
description: Uninstalls a filter with given id. Should always be called when watch isno longer needed.Additonally Filters timeout when they aren’t requested withshh_getFilterChanges for a period of time.
---

### Parameters


`id` - string

the filter id.

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
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

