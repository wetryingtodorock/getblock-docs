---
title: createmultisig  {disallowed} - Bitcoin
description: Example code for the createmultisig  {disallowed} json-rpc method. Сomplete guide on how to use createmultisig  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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

