---
title: avax:avax.issueTx \[WebSocket\] {disallowed}
description: Send a signed transaction to the network.
---

### Parameters


`tx` - string

transaction

`encoding` - string

Optional.

encoding specifies the format of the signed transaction. Can be either
"cb58" or "hex". Defaults to "cb58".

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "avax.issueTx",
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

