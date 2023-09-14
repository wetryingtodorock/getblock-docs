---
title: geth:debug_dbAncient \[POST\] {disallowed}
description: Retrieves an ancient binary blob from the freezer. The freezer is acollection of append-only immutable files.
---

### Parameters


`kind` - string

Which table to look up data from. The list of all table kinds are as
follows: headers: block headers hashes: canonical hash table (block
number -\> block hash) bodies: block bodies receipts: block receipts
diffs: total difficulty table (block number -\> td)

`number` - uint64

blob number

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_dbAncient",
"params": ["table", 1],
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

