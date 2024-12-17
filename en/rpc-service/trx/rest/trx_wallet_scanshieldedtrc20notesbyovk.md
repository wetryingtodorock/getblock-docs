---
title: trx:/wallet/scanshieldedtrc20notesbyovk  {disallowed} - TRON
description: Example code for the trx:/wallet/scanshieldedtrc20notesbyovk  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/scanshieldedtrc20notesbyovk  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`start_block_index` - int32, required.

`end_block_index` - int32, required.

`shielded_TRC20_contract_address` - string, required.

`ovk` - string, required.

`visible` - boolean

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/scanshieldedtrc20notesbyovk' \
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

