---
title: xlm:/offers \[GET\]
description: This endpoint lists all currently open offers and can be used instreaming mode. Streaming mode allows you to listen for new offers asthey are added to the Stellar ledger. If called in streaming mode,Horizon will start at the earliest known offer unless a cursor is set,in which case it will start from that cursor. By setting the cursorvalue to now, you can stream offers created since your request time.When filtering by buying or selling arguments, you must use acombination of selling_asset_type, selling_asset_issuer, andselling_asset_code for the selling asset, or a combination ofbuying_asset_type, buying_asset_issuer, and buying_asset_code for thebuying asset.
---

### Parameters


`sponser` - query

string, optional

Account ID of the sponsor. Every account in the response will either be
sponsored by the given account ID or have a subentry (trustline, offer,
or data entry) which is sponsored by the given account ID.

`seller` - query

any, optional

The account ID of the offer creator.

`selling_asset_type` - query

string, optional

The type for the selling asset. Either native, credit_alphanum4, or
credit_alphanum12.

`selling_asset_issuer` - query

any, optional

The Stellar address of the selling asset's issuer.

`selling_asset_code` - query

any, optional

The code for the selling asset.

`buying_asset_type` - query

string, optional

The type for the buying asset. Either native, credit_alphanum4, or
credit_alphanum12.

`buying_asset_issuer` - query

any, optional

The Stellar address of the buying asset's issuer.

`buying_asset_code` - query

any, optional

The code for the buying asset.

`cursor` - query

integer, optional

A number that points to a specific location in a collection of responses
and is pulled from the paging_token value of a record.

`order` - query

string, optional

A designation of the order in which records should appear. Options
include asc (ascending) or desc (descending). If this argument isn't
set, it defaults to asc.

`limit` - query

integer, optional

The maximum number of records returned. The limit can range from 1 to
200 - an upper limit that is hardcoded in Horizon for performance
reasons. If this argument isn't designated, it defaults to 10.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/offers?limit=2' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_links": {
        "self": {
            "href": "https://xlm.getblock.io/offers?cursor=&limit=2&order=asc"
        },
        "next": {
            "href": "https://xlm.getblock.io/offers?cursor=167&limit=2&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/offers?cursor=2&limit=2&order=desc"
        }
    },
    "_embedded": {
        "records": [
            {
                "_links": {
                    "self": {
                        "href": "https://xlm.getblock.io/offers/167"
                    },
                    "offer_maker": {
                        "href": "https://xlm.getblock.io/accounts/GAKC3P3LQKBRCPOQ3ACI6NHKDNHKTIPGTX7EPOC3SGCMLQK4K3WYICWK"
                    }
                },
                "id": "167",
                "paging_token": "167",
                "seller": "GAKC3P3LQKBRCPOQ3ACI6NHKDNHKTIPGTX7EPOC3SGCMLQK4K3WYICWK",
                "selling": {
                    "asset_type": "native"
                },
                "buying": {
                    "asset_type": "credit_alphanum4",
                    "asset_code": "CNY",
                    "asset_issuer": "GDOT4WJYCDEEHC6WS42OWZD2IWNJSGE64IJIQNMYFCNS4KY6A4KIZFOX"
                },
                "amount": "1.0000000",
                "price_r": {
                    "n": 1,
                    "d": 50
                },
                "price": "0.0200000",
                "last_modified_ledger": 19967410,
                "last_modified_time": null
            }
        ]
    }
}
```

