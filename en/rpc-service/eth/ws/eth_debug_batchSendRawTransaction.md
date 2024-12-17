---
title: eth:debug_batchSendRawTransaction \[WebSocket\] {disallowed}
description: Sends a list of signed transactions. This is used to quickly load anetwork with a lot of transactions. This does the same thing as callingeth_sendRawTransaction multiple times.
---

### Parameters


`data` - None

The signed transaction data array.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "debug_batchSendRawTransaction",
"params": [["0xc48fb64230a82f65a08e7280bd8745e7fea87bc7c206309dee32209fe9a985f7"]],
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

