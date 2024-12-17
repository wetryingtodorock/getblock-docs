---
title: btc:createmultisig \[POST\] {disallowed}
description: Create query m key signature multicast signature.It returns json object with address and redeem Script.
---

### Parameters


`nrequired` - number required

Number of required signatures in n keys

`keys` - json array, required

Hexadecimal public key.

`address_type` - string, optional, default = deprecated

The type of address used. The options are "deprecated"

### Request

``` java
curl --location --request POST 'https://btc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "createmultisig",
"params": [null, null, null],
"id": "getblock.io"}'
```

### Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

