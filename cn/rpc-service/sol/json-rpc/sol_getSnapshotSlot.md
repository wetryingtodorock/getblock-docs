---
title: sol:getSnapshotSlot \[POST\] {disallowed}
description: DEPRECATED Please use getHighestSnapshotSlot instead This method isexpected to be removed in solana-core v2.0Returns the highest slot that the node has a snapshot for
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://sol.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getSnapshotSlot",
"params": [],
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

