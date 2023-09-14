---
title: optimism:eth_accounts \[WebSocket\]
description: Returns a list of addresses owned by client.
---

### Parameters


\-

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
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
        "0x00000398232e2064f896018496b4b44b3d62751f"
    ]
}
```

