---
title: btg:dumpprivkey \[POST\] {disallowed}
description: Reveals the private key corresponding to ‘address’.Then the importprivkey can be used with this output
---

### Parameters


`address` - string, required

The bitcoin address for the private key

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "dumpprivkey",
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

