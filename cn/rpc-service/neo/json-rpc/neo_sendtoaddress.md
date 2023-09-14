---
title: neo:sendtoaddress \[POST\] {disallowed}
description: Transfers to the specified address.Before you can invoke this method you must call the RPC methodopenwallet to open the wallet first.
---

### Parameters


`asset_id` - string

Asset ID (asset identifier), the script hash of NEP-17 contract

`address` - string

Payment address.

`value` - string

Amount transferred.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "sendtoaddress",
"params": [null, null, null],
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

