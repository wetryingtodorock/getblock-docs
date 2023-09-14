---
title: neo:sendfrom \[POST\] {disallowed}
description: Transfer from the specified address to the destination address.Before you can invoke this method you must call the RPC methodopenwallet to open the wallet first.
---

### Parameters


`asset_id` - string

Asset ID（asset identifier）, the script hash of nep-17 contract.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "sendfrom",
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

