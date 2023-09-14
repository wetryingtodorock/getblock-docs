---
title: trx:/wallet/listexchanges \[GET\]
description: List all exchange pairs.
---

### Parameters


`visible` - boolean

### Request

``` java
curl --location --request GET 'https://trx.getblock.io/wallet/listexchanges?visible=True' \ 
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "exchanges": [
        {
            "create_time": 1615538445000,
            "creator_address": "TKEwDKE1bM6dC9Q7bvMDvwcAENc97dxQJG",
            "exchange_id": 184,
            "first_token_balance": 100000000000000,
            "first_token_id": "1003394",
            "second_token_balance": 1341470000000,
            "second_token_id": "1002922"
        },
        {
            "create_time": 1602234009000,
            "creator_address": "TYLJwXxNsrFRZyoU6KGbqxyt9rWvVLVdSu",
            "exchange_id": 183,
            "first_token_id": "1002757",
            "second_token_id": "_"
        }
    ]
}
```

