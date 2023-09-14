---
title: geth:clique_getSnapshotAtHash \[POST\] {disallowed}
description: Retrieves the state snapshot at a given block.
---

### Parameters


`blockHash` - string

block hash

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "clique_getSnapshotAtHash",
"params": ["0xfbaa33ae8b5a12bce04320f9fd609e30a300331c3d67b5ba47"],
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

