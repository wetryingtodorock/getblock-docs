---
title: shh_post  {disallowed} - KuCoin Community Chain
description: Example code for the shh_post  {disallowed} json-rpc method. Сomplete guide on how to use shh_post  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`None` - None

None

### Request

``` java
curl --location --request POST 'https://kcc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "shh_post",
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

