---
title: matic:web3_clientVersion \[WebSocket\]
description: Returns the current client version.
---

### Parameters


\-

### Request

``` java
wscat -c wss://matic.getblock.io/YOUR-API-KEY/mainnet/ 
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
    "result": "bor/v0.3.9-stable/linux-amd64/go1.19.1"
}
```

