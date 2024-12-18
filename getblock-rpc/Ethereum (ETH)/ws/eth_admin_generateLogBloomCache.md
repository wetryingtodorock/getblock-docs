---
title: admin_generateLogBloomCache  {disallowed} - Ethereum
description: Example code for the admin_generateLogBloomCache  {disallowed} ws method. Сomplete guide on how to use admin_generateLogBloomCache  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`integer` - None

Block to start generating indexes.

`integer` - None

Block to start generating indexes.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "admin_generateLogBloomCache",
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

