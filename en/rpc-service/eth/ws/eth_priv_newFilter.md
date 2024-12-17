---
title: eth:priv_newFilter \[WebSocket\] {disallowed}
description: Creates a log filter for a private contract. To poll for logs associatedwith the created filter, use priv_getFilterChanges. To get all logsassociated with the filter, use priv_getFilterLogs.For private contracts, priv_newFilter is the same as eth_newFilter forpublic contracts.
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
"method": "priv_newFilter",
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

