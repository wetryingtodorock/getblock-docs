---
title: /wallet/transferasset  {disallowed} - TRON
description: Example code for the /wallet/transferasset  {disallowed} rest method. Сomplete guide on how to use /wallet/transferasset  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

Owner address, default hexString

`to_address` - string

receiving address, default hexString

`asset_name` - string

Token id, default hexString

`amount` - int64

amount of tokens to transfer

`permission_id` - int32

Optional, for multi-signature use

`visible` - boolean

Optional, Whether the address is in base58 format.

`extra_data` - string

Optional, totes on the transaction, HEX format

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/transferasset' \
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

