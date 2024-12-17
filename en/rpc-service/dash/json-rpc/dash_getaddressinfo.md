---
title: dash:getaddressinfo \[POST\] {disallowed}
description: Returns information about the given Dash address. Note Some informationrequires the address to be in the wallet.
---

### Parameters


`Address` - string (base58)

The P2PKH or P2SH address encoded in base58check format

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getaddressinfo",
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

