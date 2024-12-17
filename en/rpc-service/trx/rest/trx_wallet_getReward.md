---
title: /wallet/getReward  {disallowed} - TRON
description: Example code for the /wallet/getReward  {disallowed} rest method. Сomplete guide on how to use /wallet/getReward  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`address` - user's address

`visible` - boolean

Optional, Whether the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getReward' \
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

