---
title: gno:eth_accounts \[WebSocket\]
description: Returns a list of account addresses a client owns.
---

### Parameters


\-

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_accounts",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        "0x8a4b7469c9c44826334f44561c5e5859a07b0123"
    ]
}
```

