---
title: theta:thetacli.ListKeys \[POST\] {disallowed}
description: This API lists the addresses of all the accounts on the local machine(i.e. under ~/.thetacli/keys/encrypted/)
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://theta.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "thetacli.ListKeys",
"params": {},
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

