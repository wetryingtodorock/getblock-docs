---
title: getaddressesbyaccount  {disallowed} - Dogecoin
description: Example code for the getaddressesbyaccount  {disallowed} json-rpc method. Сomplete guide on how to use getaddressesbyaccount  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`account` - string

Account to get list of addresses for.

### Request

``` java
curl --location --request POST 'https://doge.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getaddressesbyaccount",
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

