---
title: trx:/wallet/exchangeinject \[POST\] {disallowed}
description: Injects capital into the transaction. The purpose of injecting capitalinto the trading pair is to prevent price fluctuation from affecting thetransaction.
---

### Parameters


`owner_address` - string

Transaction to the creator's address in hexString format

`exchange_id` - int32

Transaction Pair ID

`token_id` - string

Token ID; usually is the token name, which needs to be in hexString
format.

`quant` - int32

Number of capital injection tokens.

`permission_id` - int32

Optional,for multi-signature use

`visible` - boolean

Optional,whether the address is in base58 format

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/exchangeinject' \
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

