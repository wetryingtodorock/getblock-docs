---
title: geth:personal_deriveAccount \[POST\] {disallowed}
description: Requests a HD wallet to derive a new account, optionally pinning it forlater reuse.
---

### Parameters


`url` - string

None

`path` - string

None

`pin` - string

None

### Request

``` java
curl --location --request POST 'https://geth.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "personal_deriveAccount",
"params": [null, null, null],
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

