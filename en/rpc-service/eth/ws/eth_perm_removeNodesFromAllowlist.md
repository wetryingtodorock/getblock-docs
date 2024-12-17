---
title: eth:perm_removeNodesFromAllowlist \[WebSocket\] {disallowed}
description: Removes nodes from the nodes allowlist.
---

### Parameters


`list of strings` - None

List of enode URLs

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "perm_removeNodesFromAllowlist",
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

