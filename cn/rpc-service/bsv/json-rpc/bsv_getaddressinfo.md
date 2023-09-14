---
title: bsv:getaddressinfo \[POST\] {disallowed}
description: Return information about the given bitcoin address.Some of the information will only be present if the address is in theactive wallet.
---

### Parameters


`address` - string, required

The bitcoin address for which to get information.

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getaddressinfo",
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

