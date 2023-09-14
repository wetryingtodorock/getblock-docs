---
title: eth:priv_createPrivacyGroup \[WebSocket\] {disallowed}
description: Creates a group of nodes, specified by their Orion public key.
---

### Parameters


`Object` - None

Request options

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_createPrivacyGroup",
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

