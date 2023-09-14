---
title: geth:admin_importChain \[POST\] {disallowed}
description: Imports an exported list of blocks from a local file. Importing involvesprocessing the blocks and inserting them into the canonical chain. Thestate from the parent block of this range is required.It returns a boolean indicating whether the operation succeeded.
---

### Parameters


`file` - string

adress of the local file

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "admin_importChain",
"params": ["/local/file"],
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

