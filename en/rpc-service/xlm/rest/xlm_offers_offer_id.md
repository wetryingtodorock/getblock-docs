---
title: xlm:/offers/{offer_id} \[GET\]
description: The single offer endpoint provides information on a specific offer.
---

### Parameters


`offer_id` - path

any, required

A unique identifier for this offer.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/offers/167' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_links": {
        "offer_maker": {
            "href": "https://xlm.getblock.io/accounts/GAKC3P3LQKBRCPOQ3ACI6NHKDNHKTIPGTX7EPOC3SGCMLQK4K3WYICWK"
        },
        "self": {
            "href": "https://xlm.getblock.io/offers/167"
        }
    },
    "amount": "1.0000000",
    "buying": {
        "asset_code": "CNY",
        "asset_issuer": "GDOT4WJYCDEEHC6WS42OWZD2IWNJSGE64IJIQNMYFCNS4KY6A4KIZFOX",
        "asset_type": "credit_alphanum4"
    },
    "id": "167",
    "last_modified_ledger": 19967410,
    "last_modified_time": null,
    "paging_token": "167",
    "price": "0.0200000",
    "price_r": {
        "d": 50,
        "n": 1
    },
    "seller": "GAKC3P3LQKBRCPOQ3ACI6NHKDNHKTIPGTX7EPOC3SGCMLQK4K3WYICWK",
    "selling": {
        "asset_type": "native"
    }
}
```

