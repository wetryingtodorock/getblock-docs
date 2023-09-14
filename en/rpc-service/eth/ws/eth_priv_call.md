---
title: eth:priv_call \[WebSocket\] {disallowed}
description: Invokes a private contract function locally and does not change theprivacy group state.For private contracts, priv_call is the same as eth_call for publiccontracts.
---

### Parameters


`data` - None

32-byte privacy Group ID.

`object` - None

Transaction call object.

`quantity|tag` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_call",
"params": [null, null, null],
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

