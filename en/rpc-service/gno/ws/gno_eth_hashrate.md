---
title: gno:eth_hashrate \[WebSocket\]
description: Returns the number of hashes per second with which the node is mining.When the stratum server is enabled, this method returns the cumulativehashrate of all sealers reporting their hashrate.
---

### Parameters


\-

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_hashrate",
"params": [],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0"
}
```

