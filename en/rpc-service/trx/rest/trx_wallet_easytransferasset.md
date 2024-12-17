---
title: trx:/wallet/easytransferasset \[POST\] {disallowed}
description: Easy TRC10 token transfer. Create a TRC10 transfer transaction andbroadcast directly. There is a security risk. This interface service hasbeen shutdown by the Trongrid. Please use the offline mode or the nodedeployed by yourself.
---

### Parameters


`passPhrase` - string

Password, default hexString

`toAddress` - string

To address, default hexString

`assetid` - string

Token id

`amount` - int64

Transfer token amount,the unit is the smallest unit.

`visible` - boolean

Optional, Whether the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/easytransferasset' \
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

