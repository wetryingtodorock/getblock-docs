---
title: doge:listaccounts  {disallowed} - Dogecoin
description: Example code for the doge:listaccounts  {disallowed} json-rpc method. Сomplete guide on how to use doge:listaccounts  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`minconf` - integer

Minimum number of confirmations before payments are included.

`as_dict` - boolean

Optional, default=false

Returns a dictionary of account names, with their balance as values.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "listaccounts",
"params": [1, false],
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

