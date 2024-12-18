---
title: /wallet/getBrokerage  {disallowed} - TRON
description: Example code for the /wallet/getBrokerage  {disallowed} rest method. Сomplete guide on how to use /wallet/getBrokerage  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`address` - string

Super representative's account address

`visible` - boolean

Optional, Whether the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getBrokerage' \
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

