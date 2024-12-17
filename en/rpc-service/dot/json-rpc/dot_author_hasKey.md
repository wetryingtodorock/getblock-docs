---
title: dot:author_hasKey \[POST\] {disallowed}
description: Returns true if the keystore has private keys for the given public keyand key type.
---

### Parameters


`publicKey` - Bytes

public key in bytes

`keyType` - Text

key type

### Request

``` java
curl --location --request POST 'https://dot.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "author_hasKey",
"params": ["publickeyinbytes", "keytype"],
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

