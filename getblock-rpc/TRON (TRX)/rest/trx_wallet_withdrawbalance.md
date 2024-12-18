---
title: /wallet/withdrawbalance  {disallowed} - TRON
description: Example code for the /wallet/withdrawbalance  {disallowed} rest method. Сomplete guide on how to use /wallet/withdrawbalance  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - Super representative or user address

`visible` - boolean

Optional, Whether the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/withdrawbalance' \
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

