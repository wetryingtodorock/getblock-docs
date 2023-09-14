---
title: geth:debug_standardTraceBadBlockToFile \[POST\] {disallowed}
description: This method is similar to debug_standardTraceBlockToFile, but can beused to obtain info about a block which has been rejected as invalid(for some reason).
---

### Parameters


`hash` - string

block hash

`tx` - json object

transaction hash

disableMemory - use memory of not

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_standardTraceBadBlockToFile",
"params": ["0x63a0e8e7c9e86cf58e188b98f55cedee42c3c902", {"0x263cdd926f7a8e72a3c3186f093200b3a39b7376e3ef845f66a3672e931ded3d", false}],
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

