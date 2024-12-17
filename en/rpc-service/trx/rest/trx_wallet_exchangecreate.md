---
title: /wallet/exchangecreate  {disallowed} - TRON
description: Example code for the /wallet/exchangecreate  {disallowed} rest method. Сomplete guide on how to use /wallet/exchangecreate  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

`first_token_id` - string

The first token's id, default hexString

`first_token_balance` - int32

The first token's balance

`second_token_id` - string

The second token's id, default hexString

`second_token_balance` - int32

The second token's balance

`permission_id` - int32

Optional,for multi-signature use

`visible` - boolean

Optional,whether the address is in base58 format

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/exchangecreate' \
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

