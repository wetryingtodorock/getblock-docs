---
title: doge:listunspent  {disallowed} - Dogecoin
description: Example code for the doge:listunspent  {disallowed} json-rpc method. Сomplete guide on how to use doge:listunspent  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`minconf` - integer

Minimum number of confirmations required to be listed.

`maxconf` - integer

Maximal number of confirmations allowed to be listed.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "listunspent",
"params": [1, 999999],
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

