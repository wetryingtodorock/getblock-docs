---
title: geth:debug_mutexProfile \[POST\] {disallowed}
description: Turns on mutex profiling for nsec seconds and writes profile data tofile. It uses a profile rate of 1 for most accurate information. If adifferent rate is desired, set the rate and write the profile manually.
---

### Parameters


`file` - string

address to a lical file.

`nsec` - number

profiling duration.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_mutexProfile",
"params": ["/local/file", 100],
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

