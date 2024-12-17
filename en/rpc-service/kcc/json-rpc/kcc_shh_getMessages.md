---
title: kcc:shh_getMessages  {disallowed} - KuCoin Community Chain
description: Example code for the kcc:shh_getMessages  {disallowed} json-rpc method. Сomplete guide on how to use kcc:shh_getMessages  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`id` - string

the filter id.

### Request

``` java
curl --location --request POST 'https://kcc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "shh_getMessages",
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

