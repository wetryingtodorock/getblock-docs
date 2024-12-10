---
title: dash:loadwallet  {disallowed} - Dash
description: Example code for the dash:loadwallet  {disallowed} json-rpc method. Сomplete guide on how to use dash:loadwallet  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`Filename` - string

The wallet directory or .dat file. The wallet can be specified as
file/directory basename (which must be located in the walletdir
directory), or as an absolute path to a file/directory.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "loadwallet",
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

