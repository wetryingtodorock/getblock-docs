---
title: trx:/wallet/createshieldedcontractparameters  {disallowed} - TRON
description: Example code for the trx:/wallet/createshieldedcontractparameters  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/createshieldedcontractparameters  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`ovk` - string

`from_amount` - string

`to_amount` - string

`transparent_to_address` - string

`shielded_TRC20_contract_address` - string, required

`shielded_receives` - object

`shielded_spends` - object

`ask` - string

`nsk` - string

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/createshieldedcontractparameters' \
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

