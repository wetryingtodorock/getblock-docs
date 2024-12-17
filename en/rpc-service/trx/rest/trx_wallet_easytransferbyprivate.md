---
title: trx:/wallet/easytransferbyprivate \[POST\] {disallowed}
description: Easily transfer from an address using the private key. There is asecurity risk. This interface service has been shutdown by the Trongrid.Please use the offline mode or the node deployed by yourself.
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
curl --location --request POST 'https://trx.getblock.io/wallet/easytransferbyprivate' \
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

