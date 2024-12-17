---
title: dash:backupwallet  {disallowed} - Dash
description: Example code for the dash:backupwallet  {disallowed} json-rpc method. Сomplete guide on how to use dash:backupwallet  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Destination` - string

A filename or directory name. If a filename, it will be created or
overwritten. If a directory name, the file wallet.dat will be created or
overwritten within that directory.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
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

