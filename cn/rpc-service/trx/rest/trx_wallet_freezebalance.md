---
title: trx:/wallet/freezebalance \[POST\] {disallowed}
description: Stake an amount of TRX to obtain bandwidth OR Energy and TRON Power(voting rights) . Optionally, user can stake TRX to grant Energy orBandwidth to others. Balance amount in the denomination of sun.
---

### Parameters


`owner_address` - string

Owner address, default hexString

`frozen_balance` - int64

TRX stake amount, the unit is sun

`frozen_duration` - int32

Lock-up duration for this stake, now the value can only be 3 days. It is
not allowed to unstake within 3 days after the stake. You can unstake
TRX after the 3 lock-up days

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
curl --location --request POST 'https://trx.getblock.io/wallet/freezebalance' \
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

