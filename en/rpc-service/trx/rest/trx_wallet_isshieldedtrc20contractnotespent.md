---
title: /wallet/isshieldedtrc20contractnotespent  {disallowed} - TRON
description: Example code for the /wallet/isshieldedtrc20contractnotespent  {disallowed} rest method. Сomplete guide on how to use /wallet/isshieldedtrc20contractnotespent  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`note` - object, required.

`ak` - string, required.

`nk` - string, required.

`position` - int32, required.

`shielded_TRC20_contract_address` - string, required.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/isshieldedtrc20contractnotespent' \
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

