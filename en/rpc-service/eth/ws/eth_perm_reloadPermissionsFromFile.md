---
title: eth:perm_reloadPermissionsFromFile \[WebSocket\] {disallowed}
description: Reloads the accounts and nodes allowlists from the permissionsconfiguration file.
---

### Parameters


\-

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "perm_reloadPermissionsFromFile",
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

