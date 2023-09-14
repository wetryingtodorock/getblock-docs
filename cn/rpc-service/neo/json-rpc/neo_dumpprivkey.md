---
title: neo:dumpprivkey \[POST\] {disallowed}
description: Exports the private key of the specified address.Before you can invoke this method you must call the RPC methodopenwallet to open the wallet first.
---

### Parameters


`address` - string

To export the addresses of the private key. The address is required as a
standard address.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
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

