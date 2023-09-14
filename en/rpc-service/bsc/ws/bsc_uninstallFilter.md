---
title: bsc:uninstallFilter \[WebSocket\] {disallowed}
description: Uninstalls a filter with given id. Should always be called when watch isno longer needed. Additonally Filters timeout when they arent requestedwith shh_getFilterChanges for a period of time.
---

### Parameters


`QUANTITY` - None

The filter id

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "uninstallFilter",
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

