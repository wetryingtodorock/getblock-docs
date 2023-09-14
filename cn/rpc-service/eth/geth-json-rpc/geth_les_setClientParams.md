---
title: geth:les_setClientParams \[POST\] {disallowed}
description: Set capacity and pricing factors for the specified list of connectedclients or for all connected clients if the ID list is empty.
---

### Parameters


`ids` - ids

client ids

`params` - json object

capacity and pricing factors

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "les_setClientParams",
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

