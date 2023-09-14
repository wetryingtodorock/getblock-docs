---
title: trx:/wallet/updateasset \[POST\] {disallowed}
description: Update basic TRC10 token information.
---

### Parameters


`owner_address` - string

The issuers address of the token, default hexString

`description` - string

The description of token, default hexString

`url` - string

The token's website url, default hexString

`new_limit` - int32

Each token holder's free bandwidth

`new_public_limit` - int32

The total free bandwidth of the token

`permission_id` - int32

Optional, for multi-signature use

`visible` - boolean

Optional, Whether the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/updateasset' \
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

