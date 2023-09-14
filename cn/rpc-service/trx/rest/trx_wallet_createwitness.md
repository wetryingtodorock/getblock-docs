---
title: trx:/wallet/createwitness \[POST\] {disallowed}
description: Apply to become a witness.
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

