---
title: geth:debug_getAccessibleState \[POST\] {disallowed}
description: Returns the first number where the node has accessible state on disk.This is the post-state of that block and the pre-state of the nextblock. The (from, to) parameters are the sequence of blocks to search,which can go either forwards or backwards.Note to get the last state pass in the range of blocks in reverse, i.e.(last, first).
---

### Parameters


`from` - number

block number

`to` - number

block number

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_getAccessibleState",
"params": [1, 5],
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

