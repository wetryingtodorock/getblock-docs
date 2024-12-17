---
title: etc:priv_findPrivacyGroup \[POST\] {disallowed}
description: Returns a list of privacy groups containing only the listed members. Forexample, if the listed members are A and B, a privacy group containingA, B, and C is not returned.
---

### Parameters


`array of data` - None

Members specified by Orion public keys.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_findPrivacyGroup",
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

