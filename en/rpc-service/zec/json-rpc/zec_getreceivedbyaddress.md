---
title: zec:getreceivedbyaddress \[POST\] {disallowed}
description: Returns the total amount received by the given Zcash address intransactions with at least minconf confirmations.
---

### Parameters


`zcashaddress` - string

The Zcash address for transactions.

`minconf` - numeric,

Optional, default=1

Only include transactions confirmed at least this many times.

`inZat` - boolean

Optional, default=false

Get the result amount in zatoshis (as an integer).

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getreceivedbyaddress",
"params": [null, null, null],
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

