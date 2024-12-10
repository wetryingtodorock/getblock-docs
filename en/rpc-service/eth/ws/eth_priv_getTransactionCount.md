---
title: eth:priv_getTransactionCount  {disallowed} - Ethereum
description: Example code for the eth:priv_getTransactionCount  {disallowed} ws method. Сomplete guide on how to use eth:priv_getTransactionCount  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

Account address.

`data` - None

Privacy group ID.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_getTransactionCount",
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

