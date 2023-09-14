---
title: geth:debug_setHead \[POST\] {disallowed}
description: Sets the current head of the local chain by block number. Note, this isa destructive action and may severely damage your chain. Use withextreme caution.
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
"method": "debug_setHead",
"params": [123],
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

