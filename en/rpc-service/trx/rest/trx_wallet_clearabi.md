---
title: trx:/wallet/clearabi  {disallowed} - TRON
description: Example code for the trx:/wallet/clearabi  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/clearabi  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

Owner address of the smart contract. If visible=true, use base58check
format, otherwise use hex format.

`contract_address` - string

Smart contract address. If visible=true, use base58check format,
otherwise use hex format.

`visible` - boolean

Optional. Defaults to false. Whether addresses are in base58check
format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/clearabi' \
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

