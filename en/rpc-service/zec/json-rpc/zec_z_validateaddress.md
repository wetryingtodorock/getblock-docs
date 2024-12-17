---
title: zec:z_validateaddress - Zcash
description: Example code for the zec:z_validateaddress json-rpc method. Сomplete guide on how to use zec:z_validateaddress json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`zaddr` - string

The z address to validate.

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_validateaddress",
"params": ["t1L2rjgGrvEqfrA5zqUca4GGxAeQg47CTpG"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": {
        "isvalid": false
    }
}
```

