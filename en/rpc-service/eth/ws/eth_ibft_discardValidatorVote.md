---
title: eth:ibft_discardValidatorVote \[WebSocket\] {disallowed}
description: Discards a proposal to add or remove a validator with the specifiedaddress.
---

### Parameters


`data` - None

20-byte address of proposed validator.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "ibft_discardValidatorVote",
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

