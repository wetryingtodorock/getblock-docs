---
title: /wallet/updateBrokerage  {disallowed} - TRON
description: Example code for the /wallet/updateBrokerage  {disallowed} rest method. Сomplete guide on how to use /wallet/updateBrokerage  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

Super representative's account address

`brokerage` - int32

The brokerage ratio of the super representative, for example: 20 means
20%, 100 means 100%

`visible` - boolean

Optional, Whether the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/updateBrokerage' \
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

