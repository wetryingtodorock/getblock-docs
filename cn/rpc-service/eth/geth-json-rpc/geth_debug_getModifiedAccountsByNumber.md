---
title: geth:debug_getModifiedAccountsByNumber \[POST\] {disallowed}
description: Returns all accounts that have changed between the two blocks specified.A change is defined as a difference in nonce, balance, code hash orstorage hash.
---

### Parameters


`startNum` - uint64

number of the start block

`endNum` - uint64

number of the end block

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_getModifiedAccountsByNumber",
"params": [123123, 123321],
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

