---
title: geth:miner_setRecommitInterval \[POST\] {disallowed}
description: Updates the interval for recomitting the miner sealing work.
---

### Parameters


`interval` - integer

recomitting interval

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "miner_setRecommitInterval",
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

