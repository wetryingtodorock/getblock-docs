---
title: eth:ibft_proposeValidatorVote \[WebSocket\] {disallowed}
description: Propose to add or remove a validator with the specified address.
---

### Parameters


`data` - None

Account address

`boolean` - None

true to propose adding validator or false to propose removing validator.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "ibft_proposeValidatorVote",
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

