---
title: geth:debug_setBlockProfileRate \[POST\] {disallowed}
description: Sets the rate (in samples/sec) of goroutine block profile datacollection. A non-zero rate enables block profiling, setting it to zerostops the profile. Collected profile data can be written usingdebug_writeBlockProfile.
---

### Parameters


`rate` - string

rate of data collection

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_setBlockProfileRate",
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

