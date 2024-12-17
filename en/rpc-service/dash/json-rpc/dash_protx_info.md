---
title: protx_info  {disallowed} - Dash
description: Example code for the protx_info  {disallowed} json-rpc method. Сomplete guide on how to use protx_info  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`submethod` - string

None

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "protx",
"params": ["info"],
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

