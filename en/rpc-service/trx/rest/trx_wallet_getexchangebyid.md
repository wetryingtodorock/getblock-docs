---
title: /wallet/getexchangebyid  {disallowed} - TRON
description: Example code for the /wallet/getexchangebyid  {disallowed} rest method. Сomplete guide on how to use /wallet/getexchangebyid  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`id` - int32

Transaction pair ID.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getexchangebyid' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{}'
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

