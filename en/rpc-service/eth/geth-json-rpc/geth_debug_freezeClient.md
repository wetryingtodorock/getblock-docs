---
title: geth:debug_freezeClient \[POST\] {disallowed}
description: Forces a temporary client freeze, normally when the server isoverloaded. Available as part of LES light server.
---

### Parameters


`node` - string

address of a node to freeze

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "debug_freezeClient",
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

