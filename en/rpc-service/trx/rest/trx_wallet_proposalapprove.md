---
title: trx:/wallet/proposalapprove  {disallowed} - TRON
description: Example code for the trx:/wallet/proposalapprove  {disallowed} rest method. Сomplete guide on how to use trx:/wallet/proposalapprove  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

Approver address

`proposal_id` - int32

Proposal ID

`is_add_approval` - boolean

Approved or not

`permission_id` - int32

Optional, for multi-signature use

`visible` - boolean

Optional.Whehter the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/proposalapprove' \
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

