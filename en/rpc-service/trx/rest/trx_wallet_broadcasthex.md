---
title: /wallet/broadcasthex  {disallowed} - TRON
description: Example code for the /wallet/broadcasthex  {disallowed} rest method. Сomplete guide on how to use /wallet/broadcasthex  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`transaction` - string

Transaction hex after sign

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/broadcasthex' \
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

