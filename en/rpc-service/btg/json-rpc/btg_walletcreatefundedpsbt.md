---
title: btg:walletcreatefundedpsbt \[POST\] {disallowed}
description: Creates and funds a transaction in the Partially Signed Transactionformat.Implements the Creator and Updater roles.
---

### Parameters


`inputs` - json array, optional

Leave empty to add inputs automatically. See add_inputs option.

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "walletcreatefundedpsbt",
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

