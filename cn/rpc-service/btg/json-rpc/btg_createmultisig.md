---
title: btg:createmultisig \[POST\] {disallowed}
description: Creates a multi-signature address with n signature of m keys required.It returns a json object with the address and redeemScript.
---

### Parameters


`nrequired` - numeric, required

The number of required signatures out of the n keys.

`keys` - json array, required

The hex-encoded public keys.

`address_type` - string, optional, default=legacy

The address type to use. Options are "legacy", "p2sh-segwit", and
"bech32".

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "createmultisig",
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

