---
title: eth:priv_findPrivacyGroup \[WebSocket\] {disallowed}
description: Returns a list of privacy groups containing only the listed members. Forexample, if the listed members are A and B, a privacy group containingA, B, and C is not returned.
---

### Parameters


`array of data` - None

Members specified by Orion public keys.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_findPrivacyGroup",
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

