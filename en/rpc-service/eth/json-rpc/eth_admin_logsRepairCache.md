---
title: eth:admin_logsRepairCache  {disallowed} - Ethereum
description: Example code for the eth:admin_logsRepairCache  {disallowed} json-rpc method. Сomplete guide on how to use eth:admin_logsRepairCache  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`quantity` - None

Decimal index of the starting block to fix. If left empty, the head
block is used as the starting point.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "admin_logsRepairCache",
"params": [null],
"id": "getblock.io"}'
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

