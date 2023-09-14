---
title: geth:debug_blockProfile \[POST\] {disallowed}
description: Turns on block profiling for the given duration and writes profile datato disk. It uses a profile rate of 1 for most accurate information. If adifferent rate is desired, set the rate and write the profile manuallyusing debug_writeBlockProfile.
---

### Parameters


`file` - string

local file address

`seconds` - number

block duration

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_blockProfile",
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

