---
title: avax:avax.getAtomicTx \[WebSocket\] {disallowed}
description: Gets a transaction by its ID.
---

### Parameters


`txID` - string

txID is the transacion ID. It should be in cb58 format.

`encoding` - string

Optional encoding parameter to specify the format for the returned
transaction. Can be either cb58 or hex. Defaults to cb58.

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "avax.getAtomicTx",
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

