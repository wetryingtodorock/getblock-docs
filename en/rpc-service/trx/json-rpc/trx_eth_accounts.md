---
title: trx:eth_accounts \[POST\] {disallowed}
description: Returns a list of addresses owned by the client.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/mainnet/fullnode/jsonrpc' \n--header 'x-api-key: YOUR-API-KEY' \n--header 'Content-Type: application/json' \n--data-raw '{"jsonrpc": "2.0",
"method": "eth_accounts",
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

