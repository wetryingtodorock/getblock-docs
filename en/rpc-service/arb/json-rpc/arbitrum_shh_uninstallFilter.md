---
title: shh_uninstallFilter  {disallowed} - Arbitrum
description: Example code for the shh_uninstallFilter  {disallowed} json-rpc method. Сomplete guide on how to use shh_uninstallFilter  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`id` - string

the filter id.

### Request

``` java
curl --location --request POST 'https://arbitrum.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "shh_uninstallFilter",
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

