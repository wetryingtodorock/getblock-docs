---
title: geth:debug_seedHash \[POST\] {disallowed}
description: Fetches and retrieves the seed hash of the block by number
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
"method": "debug_seedHash",
"params": [1233345],
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

