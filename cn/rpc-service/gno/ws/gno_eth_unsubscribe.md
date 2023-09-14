---
title: gno:eth_unsubscribe \[WebSocket\]
description: Cancels specified subscription. Returns true if canceled successfully orfalse otherwise.
---

### Parameters


`data` - hex string

A subscription ID previously generated with eth_subscribe method.

### Request

``` java
wscat -c wss://gno.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_unsubscribe",
"params": ["0xe5af64ddfd365b4632988c5935cfedb7"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": 1,
    "jsonrpc": "2.0",
    "result": true
}
```

