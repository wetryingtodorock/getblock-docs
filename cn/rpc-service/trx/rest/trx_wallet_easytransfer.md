---
title: trx:/wallet/easytransfer \[POST\] {disallowed}
description: Easily transfer from an address using the password string. Only workswith accounts created from createAddress,integrated getransactionsignand broadcasttransaction. There is a security risk. This interfaceservice has been shutdown by the Trongrid. Please use the offline modeor the node deployed by yourself.
---

### Parameters


`passPhrase` - string

Password converted from ascii to hex

`toAddress` - string

Recipient address converted into a hex string

`amount` - int32

Amount of TRX to transfer expressed in SUN.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/easytransfer' \
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

