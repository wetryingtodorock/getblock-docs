---
title: bch:getrawchangeaddress \[POST\] {disallowed}
description: Returns a new Bitcoin address, for receiving change.This is for use with raw transactions, NOT normal use.
---

### Parameters


`address_type` - string, optional, default=set by -changetype

The address type to use. Options are “legacy”, “p2sh-segwit”, and
“bech32”.

### Request

``` java
curl --location --request POST 'https://bch.getblock.io/mainnet/' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "getrawchangeaddress",
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

