---
title: zec:z_listreceivedbyaddress \[POST\] {disallowed}
description: Return a list of amounts received by a zaddr belonging to the nodeswallet.
---

### Parameters


`address` - string

The private address

`minconf` - numeric

Optional, default=1

Only include transactions confirmed at least this many times.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_listreceivedbyaddress",
"params": [null, null],
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

