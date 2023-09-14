---
title: eth:admin_logsRepairCache \[POST\] {disallowed}
description: Repairs cached logs by fixing all segments starting with the specifiedblock number.
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

