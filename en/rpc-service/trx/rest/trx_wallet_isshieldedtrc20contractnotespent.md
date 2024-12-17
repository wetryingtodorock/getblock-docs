---
title: trx:/wallet/isshieldedtrc20contractnotespent \[POST\] {disallowed}
description: Is Shielded Trc20 Contract Note Spent
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

