---
title: doge:getnewaddress  {disallowed} - Dogecoin
description: Example code for the doge:getnewaddress  {disallowed} json-rpc method. Сomplete guide on how to use doge:getnewaddress  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`account` - string

If account is specified (recommended), it is added to the address book
so that payments received with the address will be credited to it.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getnewaddress",
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

