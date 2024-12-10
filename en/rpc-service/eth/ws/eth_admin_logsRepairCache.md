---
title: eth:admin_logsRepairCache  {disallowed} - Ethereum
description: Example code for the eth:admin_logsRepairCache  {disallowed} ws method. Сomplete guide on how to use eth:admin_logsRepairCache  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`quantity` - None

Decimal index of the starting block to fix. If left empty, the head
block is used as the starting point.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "admin_logsRepairCache",
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

