---
title: eth:priv_distributeRawTransaction \[WebSocket\] {disallowed}
description: Distributes a signed, RLP encoded private transaction.
---

### Parameters


`data` - None

Signed RLP-encoded private transaction.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_distributeRawTransaction",
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

