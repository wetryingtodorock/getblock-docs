---
title: geth:miner_start \[POST\] {disallowed}
description: Start the CPU mining process with the given number of threads andgenerate a new DAG if need be.
---

### Parameters


`number` - number

number of threads

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "miner_start",
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

