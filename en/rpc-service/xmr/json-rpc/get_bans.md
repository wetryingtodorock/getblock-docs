---
title: xmr:get_bans  {disallowed} - Monero
description: Example code for the xmr:get_bans  {disallowed} json-rpc method. Сomplete guide on how to use xmr:get_bans  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters

\-

### Request

``` java
curl --location --request POST 'https://xmr.getblock.io/mainnet/json_rpc' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "get_bans",
"params": {},
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
