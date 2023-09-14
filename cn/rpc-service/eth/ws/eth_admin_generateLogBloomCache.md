---
title: eth:admin_generateLogBloomCache \[WebSocket\] {disallowed}
description: Generates cached log bloom indexes for blocks. APIs such as eth_getLogsand eth_getFilterLogs use the cache for improved performance.
---

### Parameters


`integer` - None

Block to start generating indexes.

`integer` - None

Block to start generating indexes.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "admin_generateLogBloomCache",
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

