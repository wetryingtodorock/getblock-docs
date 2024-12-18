---
title: /wallet/proposaldelete  {disallowed} - TRON
description: Example code for the /wallet/proposaldelete  {disallowed} rest method. Сomplete guide on how to use /wallet/proposaldelete  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

Address of proposal owner.

`proposal_id` - int32

Proposal ID

`permission_id` - int32

Optional, for multi-signature use

`visible` - boolean

Optional.Whehter the address is in base58 format.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/proposaldelete' \
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

