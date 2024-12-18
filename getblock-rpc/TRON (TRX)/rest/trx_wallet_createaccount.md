---
title: /wallet/createaccount  {disallowed} - TRON
description: Example code for the /wallet/createaccount  {disallowed} rest method. Сomplete guide on how to use /wallet/createaccount  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` -

string

Owner_address is an activated account, converted to a hex String.If the
owner_address has enough bandwidth obtained by freezing TRX, then
creating an account will only consume bandwidth , otherwise, 0.1 TRX
will be burned to pay for bandwidth, and at the same time, 1 TRX will be
required to be created.

`account_address` -

string

account_address is the address of the new account, converted to a hex
string, this address needs to be calculated in advance

`visible` -

boolean

Optional,whether the address is in base58 format

`permission_id` -

int32

Optional,for multi-signature use

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/createaccount' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"owner_address": "123QWE345F456VEBTRB567XCVE", "account_address": "SDF3BBT46YN56JS554H7J34B", "visible": "true"}'
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

