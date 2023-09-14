---
title: bsc:hasIdentity \[WebSocket\] {disallowed}
description: Checks if the client hold the private keys for a given identity.
---

### Parameters


`DATA` - None

60 Bytes - The identity address to check.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "hasIdentity",
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

