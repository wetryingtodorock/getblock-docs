---
title: dash:rescanblockchain \[POST\] {disallowed}
description: Rescans the local blockchain for wallet related transactions.
---

### Parameters


`Start Height` - integer

Optional.

The block height where the rescan should start.

`Stop Height` - integer

Optional.

The last block height that should be scanned.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "rescanblockchain",
"params": [null, null],
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

