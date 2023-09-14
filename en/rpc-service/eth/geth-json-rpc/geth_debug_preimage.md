---
title: geth:debug_preimage \[POST\] {disallowed}
description: Returns the preimage for a sha3 hash, if known.
---

### Parameters


`hash` - string

sha3 hash

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_preimage",
"params": ["003BE8bd8dBa04Ac4dE888A9ea02AcF73b61700"],
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

