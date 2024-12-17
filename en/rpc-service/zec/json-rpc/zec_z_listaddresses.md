---
title: zec:z_listaddresses  {disallowed} - Zcash
description: Example code for the zec:z_listaddresses  {disallowed} json-rpc method. Сomplete guide on how to use zec:z_listaddresses  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`includeWatchonly` - boolean

Optional, default=false

Also include watchonly addresses.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_listaddresses",
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

