---
title: z_listoperationids  {disallowed} - Zcash
description: Example code for the z_listoperationids  {disallowed} json-rpc method. Сomplete guide on how to use z_listoperationids  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`status` - string

Optional.

Filter result by the operation's state e.g. "success".

### Request

``` java
curl --location --request POST 'https://zec.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "z_listoperationids",
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

