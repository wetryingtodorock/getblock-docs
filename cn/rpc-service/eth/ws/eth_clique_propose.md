---
title: eth:clique_propose \[WebSocket\] {disallowed}
description: Propose to add or remove a signer with the specified address.
---

### Parameters


`data` - None

20-byte address.

`boolean` - None

true to propose adding signer or false to propose removing signer.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "clique_propose",
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

