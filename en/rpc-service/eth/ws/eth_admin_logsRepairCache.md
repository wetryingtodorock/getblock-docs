---
title: eth:admin_logsRepairCache \[WebSocket\] {disallowed}
description: Repairs cached logs by fixing all segments starting with the specifiedblock number.
---

### Parameters


`quantity` - None

Decimal index of the starting block to fix. If left empty, the head
block is used as the starting point.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "admin_logsRepairCache",
"params": [null],
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

