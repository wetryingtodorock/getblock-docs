---
title: eth:priv_getLogs \[WebSocket\] {disallowed}
description: Returns an array of logs matching a specified filter object.For private contracts, priv_getLogs is the same as eth_getLogs forpublic contracts except there is no automatic log bloom caching forprivate contracts.
---

### Parameters


`data` - None

32-byte privacy Group ID.

`Object` - None

Filter options object.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_getLogs",
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

