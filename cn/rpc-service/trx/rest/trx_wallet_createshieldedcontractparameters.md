---
title: trx:/wallet/createshieldedcontractparameters \[POST\] {disallowed}
description: Note To ensure security, Trongrid has disabled this interface service,please use the service provided by the local node.
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

