---
title: db_getString  {disallowed} - KuCoin Community Chain
description: Example code for the db_getString  {disallowed} json-rpc method. Сomplete guide on how to use db_getString  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`database` - string

database name

`key` - string

key name

### Request

``` java
curl --location --request POST 'https://kcc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "db_getString",
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
