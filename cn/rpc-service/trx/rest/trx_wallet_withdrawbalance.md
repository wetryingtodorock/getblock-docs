---
title: trx:/wallet/withdrawbalance \[POST\] {disallowed}
description: Super Representative or user withdraw rewards, usable every 24 hours.Super representatives can withdraw the balance from the accountallowance into the account balance, Users can claim the voting rewardfrom the SRs and deposit into his account balance.
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

