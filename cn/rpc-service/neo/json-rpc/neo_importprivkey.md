---
title: neo:importprivkey \[POST\] {disallowed}
description: Imports the private key to the wallet.Before you can invoke this method you must call the RPC methodopenwallet to open the wallet first.
---

### Parameters


`key` - string

The WIF-format private key.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "importprivkey",
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

