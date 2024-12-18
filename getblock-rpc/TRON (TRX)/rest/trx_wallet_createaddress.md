---
title: /wallet/createaddress  {disallowed} - TRON
description: Example code for the /wallet/createaddress  {disallowed} rest method. Сomplete guide on how to use /wallet/createaddress  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`value` - string, required

value is the password, converted from ascii to hex. i.e. the pass
phrase.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/createaddress' \
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

