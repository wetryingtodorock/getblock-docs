---
title: trx:/wallet/updatewitness  {disallowed} - TRON
description: Example code for the trx:/wallet/updatewitness  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/updatewitness  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

Owner address, default hexString

`update_url` - string

Website url, default hexString

`permission_id` - int32

Optional, for multi-signature use

`visible` - boolean

Optional, Whether the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/updatewitness' \
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

