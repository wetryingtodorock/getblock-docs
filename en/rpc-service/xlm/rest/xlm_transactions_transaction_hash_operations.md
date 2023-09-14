---
title: xlm:/transactions/{transaction_hash}/operations \[GET\]
description: This endpoint returns Successful operations for a specific transaction.
---

### Parameters


`transaction_hash` - path

string, required

Transactions are commands that modify the ledger state and consist of
one or more operations.

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

`include_fail` - query

boolean, optional

Set to true to include failed operations in results. Options include
true and false.

`join` - query

any, optional

Set to transactions to include the transactions which created each of
the operations in the response.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet//transactions/339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601/operations?limit=1' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_embedded": {
        "records": [
            {
                "_links": {
                    "effects": {
                        "href": "https://xlm.getblock.io/operations/196188608523145217/effects"
                    },
                    "precedes": {
                        "href": "https://xlm.getblock.io/effects?order=asc&cursor=196188608523145217"
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/operations/196188608523145217"
                    },
                    "succeeds": {
                        "href": "https://xlm.getblock.io/effects?order=desc&cursor=196188608523145217"
                    },
                    "transaction": {
                        "href": "https://xlm.getblock.io/transactions/339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601"
                    }
                },
                "amount": "676.8606311",
                "buying_asset_type": "native",
                "created_at": "2023-04-04T10:14:50Z",
                "id": "196188608523145217",
                "offer_id": "1213948452",
                "paging_token": "196188608523145217",
                "price": "0.1748437",
                "price_r": {
                    "d": 502234256,
                    "n": 87812489
                },
                "selling_asset_code": "ONEH",
                "selling_asset_issuer": "GBRYUM4VAR3ZVR5UJREOEX5NQJRUD7CJD5EK7GWVFYI4FBD4JPZJ4EBK",
                "selling_asset_type": "credit_alphanum4",
                "source_account": "GBCMDTXXKTTPTIUBQ3UEDVRI5KXKZZ2JDR7S2WBL2CIIUYI5PPU5ZWP7",
                "transaction_hash": "339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601",
                "transaction_successful": true,
                "type": "manage_sell_offer",
                "type_i": 3
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/transactions/339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601/operations?cursor=196188608523145217&limit=2&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/transactions/339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601/operations?cursor=196188608523145217&limit=2&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/transactions/339a5de63a8a0b0224b30e9e17243ae52785b24402db003090c73a862eafc601/operations?cursor=&limit=2&order=asc"
        }
    }
}
```

