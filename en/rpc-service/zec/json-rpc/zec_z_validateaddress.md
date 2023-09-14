---
title: zec:z_validateaddress \[POST\]
description: Return information about the given z address.
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

