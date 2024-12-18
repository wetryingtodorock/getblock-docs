---
title: priv_getCode  {disallowed} - Ethereum
description: Example code for the priv_getCode  {disallowed} ws method. Сomplete guide on how to use priv_getCode  {disallowed} ws in GetBlock.io Web3 documentation.
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

