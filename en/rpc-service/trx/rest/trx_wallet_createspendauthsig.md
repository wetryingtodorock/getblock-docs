---
title: trx:/wallet/createspendauthsig  {disallowed} - TRON
description: Example code for the trx:/wallet/createspendauthsig  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/createspendauthsig  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`ask` - string, required.

`tx_hash` - string, required.

`aplha` - string, required.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/createspendauthsig' \
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

