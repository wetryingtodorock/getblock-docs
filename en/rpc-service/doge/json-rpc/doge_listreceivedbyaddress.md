---
title: doge:listreceivedbyaddress  {disallowed} - Dogecoin
description: Example code for the doge:listreceivedbyaddress  {disallowed} json-rpc method. Сomplete guide on how to use doge:listreceivedbyaddress  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`minconf` - integer

Minimum number of confirmations before payments are included.

`includeempty` - boolean

Optional, default=false

Whether to include addresses that haven’t received any payments.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "listreceivedbyaddress",
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

