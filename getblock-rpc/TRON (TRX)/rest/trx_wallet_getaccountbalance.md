---
title: /wallet/getaccountbalance  {disallowed} - TRON
description: Example code for the /wallet/getaccountbalance  {disallowed} rest method. Сomplete guide on how to use /wallet/getaccountbalance  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`account_identifier` - json object

`block_identifier` - json object

`visible` - boolean

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getaccountbalance' \
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

