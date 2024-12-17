---
title: eth:priv_uninstallFilter \[WebSocket\] {disallowed}
description: Uninstalls a filter for a private contract with the specified ID. When afilter is no longer required, call this method.Filters time out when not requested by priv_getFilterChanges orpriv_getFilterLogs for 10 minutes.For private contracts, priv_uninstallFilter is the same aseth_uninstallFilter for public contracts.
---

### Parameters


`data` - None

32-byte privacy Group ID.

`data` - None

Filter ID.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_uninstallFilter",
"params": [null, null],
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

