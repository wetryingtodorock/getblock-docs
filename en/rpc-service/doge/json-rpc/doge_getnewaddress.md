---
title: doge:getnewaddress \[POST\] {disallowed}
description: Returns a new dogecoin address for receiving payments.
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

