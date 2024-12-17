---
title: trx:/wallet/createwitness  {disallowed} - TRON
description: Example code for the trx:/wallet/createwitness  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/createwitness  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

Owner address, default hexString

`url` - string

Website url, default hexString

`permission_id` - int32

Optional, for multi-signature use

`visible` - boolean

Optional, Whether the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/createwitness' \
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

