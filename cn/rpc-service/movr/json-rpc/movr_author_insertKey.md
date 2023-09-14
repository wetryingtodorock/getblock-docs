---
title: movr:author_insertKey \[POST\] {disallowed}
description: Insert a key into the keystore.
---

### Parameters


`keyType` - Text

key type

`suri` - Text

suri

`publicKey` - Bytes

public key

### Request

``` java
curl --location --request POST 'https://movr.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "author_insertKey",
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

