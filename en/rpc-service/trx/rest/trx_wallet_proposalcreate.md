---
title: trx:/wallet/proposalcreate \[POST\] {disallowed}
description: Creates a proposal transaction.
---

### Parameters


`owner_address` - string

Address of the transaction creator

`parameters` - json object

Proposal parameters

`permission_id` - int32

Optional, for multi-signature use

`visible` - boolean

Optional.Whehter the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/proposalcreate' \
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

