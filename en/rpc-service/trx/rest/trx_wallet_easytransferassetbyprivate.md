---
title: trx:/wallet/easytransferassetbyprivate \[POST\] {disallowed}
description: TRC10 token easy transfer. Broadcast the created transaction directly.There is a security risk. This interface service has been shutdown bythe Trongrid. Please use the offline mode or the node deployed byyourself.
---

### Parameters


`privateKey` - string

Private key, default hexString

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
curl --location --request POST 'https://trx.getblock.io/wallet/easytransferassetbyprivate' \
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

