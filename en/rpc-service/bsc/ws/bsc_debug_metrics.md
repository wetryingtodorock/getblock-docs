---
title: bsc:debug_metrics \[WebSocket\] {disallowed}
description: Returns metrics providing information on the internal operation of Besu.The available metrics might change over time. The JVM metrics might varybased on the JVM implementation used.
---

### Parameters


\-

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_metrics",
"params": [],
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

