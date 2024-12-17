---
title: eth:admin_nodeInfo \[WebSocket\] {disallowed}
description: Returns networking information about the node. The information includesgeneral information about the node and specific information from eachrunning Ethereum sub-protocol (for example, eth).
---

### Parameters


\-

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "admin_nodeInfo",
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

