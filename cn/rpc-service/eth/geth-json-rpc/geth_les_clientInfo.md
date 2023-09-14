---
title: geth:les_clientInfo \[POST\] {disallowed}
description: Get individual client information (connection, balance, pricing) on thespecified list of clients or for all connected clients if the ID list isempty.
---

### Parameters


`ids` - array of json object

Optional. List of client id.

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "les_clientInfo",
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

