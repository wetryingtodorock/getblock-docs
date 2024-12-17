---
title: eth:priv_getTransactionReceipt \[WebSocket\] {disallowed}
description: Returns information about the private transaction after mining thetransaction. Receipts for pending transactions are not available.
---

### Parameters


`data` - None

32-byte hash of a transaction.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_getTransactionReceipt",
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

