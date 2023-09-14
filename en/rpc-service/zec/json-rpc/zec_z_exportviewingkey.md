---
title: zec:z_exportviewingkey \[POST\] {disallowed}
description: Reveals the viewing key corresponding to zaddr. Then thez_importviewingkey can be used with this output
---

### Parameters


`zaddr` - string

The zaddr for the private key.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_exportviewingkey",
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

