---
title: trx:/wallet/unfreezebalance \[POST\] {disallowed}
description: Unstake TRX that has passed the minimum stake duration to releasebandwidth and energy and at the same time TRON Power will reduce and allvotes will be canceled.
---

### Parameters


`owner_address` - string

Owner address, default hexString

`resource` - string

TRX stake type, 'BANDWIDTH' or 'ENERGY'

`recelver_address` - string

Optional,the address that will receive the resource, default hexString

`permission_id` - int32

Optional, for multi-signature use

`visible` - boolean

Optional. Defaults to false. Whether addresses are in base58check
format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/unfreezebalance' \
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

