---
title: trx:/wallet/getcontract \[POST\] {disallowed}
description: Queries a contracts information from the blockchain, including thebytecode of the contract, ABI, configuration parameters, etc.
---

### Parameters


`value` - string

Contract address, converted to a hex string.

`visible` - boolean

Optional, is address in visible format(base58check) or hex?

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getcontract' \
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

