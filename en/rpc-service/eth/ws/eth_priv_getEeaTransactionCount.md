---
title: eth:priv_getEeaTransactionCount  {disallowed} - Ethereum
description: Example code for the eth:priv_getEeaTransactionCount  {disallowed} ws method. Сomplete guide on how to use eth:priv_getEeaTransactionCount  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

Account address.

`data` - None

Base64 encoded Orion address of the sender.

`array of data` - None

Base64 encoded Orion addresses of recipients.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_getEeaTransactionCount",
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

