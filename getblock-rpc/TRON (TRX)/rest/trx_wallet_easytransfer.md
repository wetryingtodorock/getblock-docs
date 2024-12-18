---
title: /wallet/easytransfer  {disallowed} - TRON
description: Example code for the /wallet/easytransfer  {disallowed} rest method. Сomplete guide on how to use /wallet/easytransfer  {disallowed} rest in GetBlock.io Web3 documentation.
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

