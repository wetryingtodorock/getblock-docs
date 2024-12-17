---
title: bch:invalidateblock \[POST\] {disallowed}
description: Permanently marks a block as invalid, as if it violated a consensusrule.
---

### Parameters


`blockhash` - string, required

the hash of the block to mark as invalid

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "invalidateblock",
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

