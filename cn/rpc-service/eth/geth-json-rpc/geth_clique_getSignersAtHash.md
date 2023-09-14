---
title: geth:clique_getSignersAtHash \[POST\] {disallowed}
description: Retrieves the list of authorized signers at the specified block hash.
---

### Parameters


`blockHash` - string

block hash

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "clique_getSignersAtHash",
"params": ["0xfbaa33ae8b5a12bce04320f9fd609e30a300331c"],
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

