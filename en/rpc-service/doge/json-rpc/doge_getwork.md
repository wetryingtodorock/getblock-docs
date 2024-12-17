---
title: doge:getwork  {disallowed} - Dogecoin
description: Example code for the doge:getwork  {disallowed} json-rpc method. Сomplete guide on how to use doge:getwork  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`data` - string

Optional.

Result from remote mining.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getwork",
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

