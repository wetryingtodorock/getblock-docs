---
title: geth:admin_exportChain \[POST\] {disallowed}
description: Exports the current blockchain into a local file. It optionally takes afirst and last block number, in which case it exports only that range ofblocks.It returns a boolean indicating whether the operation succeeded.
---

### Parameters


`file` - string

Adress of the local file.

`start` - uint64

Optional.

First block to be exported.

`finish` - uint64

Optional.

Last block to be exported.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "admin_exportChain",
"params": ["/local/file", 1, 5],
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

