---
title: bsv:generateblock \[POST\] {disallowed}
description: Mine a block with a set of ordered transactions immediately to aspecified address or descriptor (before the RPC call returns)
---

### Parameters


`output` - string, required

The address or descriptor to send the newly generated btc to.

`transactions` - json array, required

An array of hex strings which are either txids or raw transactions.

Txids must reference transactions currently in the mempool.

All transactions must be valid and in valid order, otherwise the block
will be rejected.

### Request

``` java
curl --location --request POST 'https://bsv.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "generateblock",
"params": [null, null],
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

