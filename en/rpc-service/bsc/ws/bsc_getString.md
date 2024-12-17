---
title: bsc:getString \[WebSocket\] {disallowed}
description: Returns string from the local database.Note this function is deprecated and will be removed in the future.
---

### Parameters


`String` - None

Database name

`String` - None

Key name

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "getString",
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

