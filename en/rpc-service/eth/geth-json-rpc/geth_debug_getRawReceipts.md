---
title: geth:debug_getRawReceipts \[POST\] {disallowed}
description: Returns the consensus-encoding of all receipts in a single block.
---

### Parameters


`blockNrOrHash` - string

block number or hash

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_getRawReceipts",
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

