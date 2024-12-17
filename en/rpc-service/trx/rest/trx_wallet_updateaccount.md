---
title: /wallet/updateaccount  {disallowed} - TRON
description: Example code for the /wallet/updateaccount  {disallowed} rest method. Сomplete guide on how to use /wallet/updateaccount  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`account_name` -

string

Account_name is the name of the account, converted to a hex string

`owner_address` -

string

Owner_address is the account address to be modified, converted to a hex
string

`visible` -

boolean

Optional,whether the address is in base58 format

`permission_id` -

int32

Optional,for multi-signature use

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/updateaccount' \
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

