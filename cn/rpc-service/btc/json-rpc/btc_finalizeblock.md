---
title: btc:finalizeblock \[POST\] {disallowed}
description: Treats a block as final. It cannot be reorged.Any chain that does not contain this block is invalid.Used on a less work chain, it can effectively PUTS YOU OUT OF CONSENSUS.USE WITH CAUTION!
---

### Parameters


`blockhash` - string, required

the hash of the block

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "finalizeblock",
"params": [null],
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

