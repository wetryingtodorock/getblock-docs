---
title: doge:backupwallet  {disallowed} - Dogecoin
description: Example code for the doge:backupwallet  {disallowed} json-rpc method. Сomplete guide on how to use doge:backupwallet  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`destination` - string

directory or path with filename to backup wallet to.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "backupwallet",
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

