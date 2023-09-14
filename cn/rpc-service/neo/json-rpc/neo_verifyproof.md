---
title: neo:verifyproof \[POST\] {disallowed}
description: Verifies using the root hash and proof, and gets the value of thestorage corresponding to the key.
---

### Parameters


`roothash` - string

root hash of the state root

`proof` - string

proof data of the state root; Base64-encoded.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "verifyproof",
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

