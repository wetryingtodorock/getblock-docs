---
title: trx:/wallet/accountpermissionupdate  {disallowed} - TRON
description: Example code for the trx:/wallet/accountpermissionupdate  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/accountpermissionupdate  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` -

string

`actives` -

array of json objects

`owner` -

json object

`witness` -

json object

`visible` -

boolean

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/accountpermissionupdate' \ 
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

