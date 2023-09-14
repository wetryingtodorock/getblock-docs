---
title: geth:debug_getBlockRlp \[POST\] {disallowed}
description: Retrieves and returns the RLP encoded block by number.
---

### Parameters


`number` - uint64

block number

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_getBlockRlp",
"params": [123123],
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

