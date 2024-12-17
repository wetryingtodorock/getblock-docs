---
title: zec:z_exportkey \[POST\] {disallowed}
description: Reveals the zkey corresponding to zaddr. Then the z_importkey can beused with this output.
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
"method": "z_exportkey",
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

