---
title: geth:clique_getSnapshot \[POST\] {disallowed}
description: Retrieves a snapshot of all clique state at a given block.
---

### Parameters


`blockNumber` - integer

block number

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "clique_getSnapshot",
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

