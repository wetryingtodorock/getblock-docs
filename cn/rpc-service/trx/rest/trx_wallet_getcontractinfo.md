---
title: trx:/wallet/getcontractinfo \[POST\] {disallowed}
description: Queries a contracts information from the blockchain. The differencefrom the wallet/getcontract interface is that this interface returns notonly the bytecode but also the runtime bytecode of the contract.Compared with bytecode, runtime bytecode does not contain constructorand constructor parameter information.
---

### Parameters


`value` - string

Contract address, converted to a hex string.

`visible` - boolean

Optional, is address in visible format(base58check) or hex?

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getcontractinfo' \
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

