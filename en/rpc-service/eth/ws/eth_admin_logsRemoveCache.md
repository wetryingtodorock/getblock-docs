---
title: eth:admin_logsRemoveCache \[WebSocket\] {disallowed}
description: Removes cache files for the specified range of blocks.
---

### Parameters


`fromBlock` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

`toBlock` - None

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "admin_logsRemoveCache",
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

