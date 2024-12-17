---
title: zec:getgenerate \[POST\] {disallowed}
description: Return if the server is set to generate coins or not. The default isfalse.It is set with the command line argument -gen (or zcash.conf settinggen)It can also be set with the setgenerate call.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getgenerate",
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

