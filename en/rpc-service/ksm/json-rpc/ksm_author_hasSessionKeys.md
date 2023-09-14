---
title: ksm:author_hasSessionKeys \[POST\] {disallowed}
description: Returns true if the keystore has private keys for the given sessionpublic keys.
---

### Parameters


`sessionKeys` - Bytes

session keys in bytes

### Request

``` java
curl --location --request POST 'https://ksm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "author_hasSessionKeys",
"params": ["sessionkeysinbytes"],
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

