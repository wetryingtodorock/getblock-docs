---
title: priv_uninstallFilter  {disallowed} - Ethereum Classic
description: Example code for the priv_uninstallFilter  {disallowed} json-rpc method. Сomplete guide on how to use priv_uninstallFilter  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

32-byte privacy Group ID.

`data` - None

Filter ID.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "priv_uninstallFilter",
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
