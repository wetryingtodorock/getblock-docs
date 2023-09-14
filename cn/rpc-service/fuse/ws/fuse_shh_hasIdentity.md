---
title: fuse:shh_hasIdentity \[WebSocket\] {disallowed}
description: Checks if the client hold the private keys for a given identity.
---

### Parameters


`address` - data

the address of the new identiy.

### Request

``` java
wscat -c wss://fuse.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "shh_hasIdentity",
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

