---
title: eth:priv_getTransactionReceipt  {disallowed} - Ethereum
description: Example code for the eth:priv_getTransactionReceipt  {disallowed} ws method. Сomplete guide on how to use eth:priv_getTransactionReceipt  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

32-byte hash of a transaction.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "priv_getTransactionReceipt",
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

