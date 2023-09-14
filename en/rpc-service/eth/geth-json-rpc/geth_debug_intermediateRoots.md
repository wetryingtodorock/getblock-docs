---
title: geth:debug_intermediateRoots \[POST\] {disallowed}
description: Executes a block (bad- or canon- or side-), and returns a list ofintermediate roots the stateroot after each transaction.
---

### Parameters


`blockHash` - string

hash of the block

`options` - array of string

additional options

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_intermediateRoots",
"params": ["0x0003BE8bd8dBa04Ac4dE888A9ea02AcF73b61700"],
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

