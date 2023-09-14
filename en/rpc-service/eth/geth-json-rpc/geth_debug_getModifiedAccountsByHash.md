---
title: geth:debug_getModifiedAccountsByHash \[POST\] {disallowed}
description: Returns all accounts that have changed between the two blocks specified.A change is defined as a difference in nonce, balance, code hash, orstorage hash. With one parameter, returns the list of accounts modifiedin the specified block.
---

### Parameters


`startHash` - string

hash of the start block

`endHash` - string

hash of the end block

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_getModifiedAccountsByHash",
"params": ["0x000251bd7762a21df45175e6e571e83f68d15f3e", "0x0003BE8bd8dBa04Ac4dE888A9ea02AcF73b61700"],
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

