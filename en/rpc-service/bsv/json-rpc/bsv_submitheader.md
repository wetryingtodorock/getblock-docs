---
title: bsv:submitheader \[POST\] {disallowed}
description: Decode the given hexdata as a header and submit it as a candidate chaintip if valid.Throws when the header is invalid.
---

### Parameters


`hexdata` - string, required

The hex-encoded block header data

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "submitheader",
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

