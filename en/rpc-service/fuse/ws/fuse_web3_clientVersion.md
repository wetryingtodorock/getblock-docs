---
title: fuse:web3_clientVersion \[WebSocket\]
description: Returns the current client version.
---

### Parameters


\-

### Request

``` java
wscat -c wss://fuse.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "web3_clientVersion",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "OpenEthereum//v3.3.5-stable/x86_64-linux-musl/rustc1.59.0"
}
```

