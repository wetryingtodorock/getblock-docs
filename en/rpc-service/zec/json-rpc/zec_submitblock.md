---
title: submitblock  {disallowed} - Zcash
description: Example code for the submitblock  {disallowed} json-rpc method. Сomplete guide on how to use submitblock  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`hexdata` - string

the hex-encoded block data to submit

`jsonparametersobject` - string

Optional, currently ignored.

object of optional parameters

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "submitblock",
"params": [null, null],
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

