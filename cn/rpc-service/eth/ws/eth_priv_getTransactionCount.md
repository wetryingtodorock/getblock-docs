---
title: eth:priv_getTransactionCount \[WebSocket\] {disallowed}
description: Returns the private transaction count for specified account and privacygroup.
---

### Parameters


`data` - None

Account address.

`data` - None

Privacy group ID.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_getTransactionCount",
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

