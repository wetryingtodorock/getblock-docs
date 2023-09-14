---
title: geth:miner_setGasPrice \[POST\] {disallowed}
description: Sets the minimal accepted gas price when mining transactions. Anytransactions that are below this limit are excluded from the miningprocess.
---

### Parameters


`number` - number

minimal accepted gas price

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "miner_setGasPrice",
"params": [1],
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

