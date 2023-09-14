---
title: neo:getproof \[POST\] {disallowed}
description: Gets proof by querying root hash, contract hash, and storage key.
---

### Parameters


`roothash` - string

Root hash of state root.

`scripthash` - string

Contract script hash.

`key` - string

Key of the storage; Base64-encoded.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getproof",
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

