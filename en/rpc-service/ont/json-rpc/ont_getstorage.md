---
title: ont:getstorage \[POST\]
description: Fetched the stored value using contract hash and the storage key. Resultwill be hex string.
---

### Parameters


`hash` - string

contract hash

`key` - integer

storage key

The storage key is a hexadecimal string.

### Request

``` java
curl --location --request POST 'https://ont.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getstorage",
"params": ["03febccf81ac85e3d795bc5cbd4e84e907812aa3", "5065746572"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "desc": "SUCCESS",
    "error": 0,
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": null
}
```

