---
title: eth:ibft_getSignerMetrics \[WebSocket\] {disallowed}
description: Provides validator metrics for the specified range
---

### Parameters


`fromBlockNumber` - None

Integer representing a block number or the string tag earliest as
described in Block Parameter.

`toBlockNumber` - None

Integer representing a block number or one of the string tags latest or
pending, as described in Block Parameter

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "ibft_getSignerMetrics",
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

