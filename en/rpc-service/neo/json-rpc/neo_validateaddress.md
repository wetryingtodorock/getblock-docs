---
title: neo:validateaddress \[POST\]
description: Verifies that the address is a valid NEO address.
---

### Parameters


`address` - string

Address. The NEO standard address begins with N because AddressVersion
in Neo N3 has been modified to 53.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "validateaddress",
"params": ["NPvKVTGZapmFWABLsyvfreuqn73jCjJtN1"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": {
        "address": "NPvKVTGZapmFWABLsyvfreuqn73jCjJtN1",
        "isvalid": true
    },
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

