---
title: /wallet/exchangetransaction  {disallowed} - TRON
description: Example code for the /wallet/exchangetransaction  {disallowed} rest method. Сomplete guide on how to use /wallet/exchangetransaction  {disallowed} rest in GetBlock.io Web3 documentation.
---

### Parameters


`owner_address` - string

Trader's wallet address, in hex string format. This wallet contains the
tokens you wish to sell, in order to gain the other token.

`exchange_id` - int32

Transaction Pair ID

`token_id` - string

ID of the sold token, in hexString format. For example, if you wanted to
trade TRX for another token, then the TRX id of "5f" goes in this
parameter.

`quant` - int32

Quantity of the token being sold. If TRX being sold, need to express in
units of SUN.

`expected` - int32

Expected quantity of the token being purchased.

`permission_id` - int32

Optional,for multi-signature use

`visible` - boolean

Optional,whether the address is in base58 format

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/exchangetransaction' \
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

