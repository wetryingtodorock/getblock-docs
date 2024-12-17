---
title: dash:importwallet \[POST\] {disallowed}
description: Imports private keys from a file in wallet dump file format (see thedumpwallet RPC). These keys will be added to the keys currently in thewallet. This call may need to rescan all or parts of the block chain fortransactions affecting the newly-added keys, which may take severalminutes.
---

### Parameters


`Filename` - string

The file to import. The path is relative to Dash Core's working
directory.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "importwallet",
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

