---
title: zec:settxfee \[POST\] {disallowed}
description: Set the transaction fee per kB. Overwrites the paytxfee parameter.
---

### Parameters


`amount` - numeric

The transaction fee in ZEC/kB rounded to the nearest 0.00000001

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "settxfee",
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

