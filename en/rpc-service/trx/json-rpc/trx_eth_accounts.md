---
title: trx:eth_accounts  {disallowed} - TRON
description: Example code for the trx:eth_accounts  {disallowed} json-rpc method. Сomplete guide on how to use trx:eth_accounts  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/mainnet/jsonrpc' \n--header 'x-api-key: YOUR-API-KEY' \n--header 'Content-Type: application/json' \n--data-raw '{"jsonrpc": "2.0",
"method": "eth_accounts",
"params": [],
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

