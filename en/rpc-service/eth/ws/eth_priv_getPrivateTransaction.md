---
title: eth:priv_getPrivateTransaction \[WebSocket\] {disallowed}
description: Returns the private transaction if you are a participant, otherwise,null.
---

### Parameters


`data` - None

Transaction hash returned by eea_sendRawTransaction or
eea_sendTransaction.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_getPrivateTransaction",
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

