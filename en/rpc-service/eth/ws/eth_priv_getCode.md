---
title: eth:priv_getCode \[WebSocket\] {disallowed}
description: Returns the code of the private smart contract at the specified address.Compiled smart contract code is stored as a hexadecimal value.
---

### Parameters


`data` - None

32-byte privacy Group ID.

`data` - None

20-byte contract address.

`quantity|tag` - None

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_getCode",
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

