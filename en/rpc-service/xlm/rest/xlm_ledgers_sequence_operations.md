---
title: xlm:/ledgers/{sequence}/operations \[GET\]
description: This endpoint returns all payment-related operations in a specificledger. Operation types that can be returned by this endpoint includecreate_account, payment, path_payment, and account_merge.
---

### Parameters


`sequence` - path

integer, optional

The sequence number of a specific ledger.

`cursor` - query

integer, optional

A number that points to a specific location in a collection of responses
and is pulled from the paging_token value of a record.

`order` - query

string, optional

A designation of the order in which records should appear. Options
include asc (ascending) or desc (descending). If this argument isn’t
set, it defaults to asc.

`limit` - query

integer, optional

The maximum number of records returned. The limit can range from 1 to
200 - an upper limit that is hardcoded in Horizon for performance
reasons. If this argument isn’t designated, it defaults to 10.

`include_failed` - query

boolean, optional

Set to true to include failed operations in results. Options include
true and false.

`join` - query

any, optional

Set to transactions to include the transactions which created each of
the operations in the response.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/ledgers/45678721/operations?limit=1' 
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
                        "href": "https://xlm.getblock.io/operations/196188612818112514/effects"
                    },
                    "precedes": {
                        "href": "https://xlm.getblock.io/effects?order=asc&cursor=196188612818112514"
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/operations/196188612818112514"
                    },
                    "succeeds": {
                        "href": "https://xlm.getblock.io/effects?order=desc&cursor=196188612818112514"
                    },
                    "transaction": {
                        "href": "https://xlm.getblock.io/transactions/0a33e149a21b67e11fabb30e41adb08984766550f0e83bd2ae66b33a183dd452"
                    }
                },
                "amount": "10000000000.0000000",
                "buying_asset_type": "native",
                "created_at": "2023-04-04T10:14:56Z",
                "id": "196188612818112514",
                "offer_id": "0",
                "paging_token": "196188612818112514",
                "price": "0.0000001",
                "price_r": {
                    "d": 10000000,
                    "n": 1
                },
                "selling_asset_code": "STEEL",
                "selling_asset_issuer": "GBV4NISN6Y4PIB3JRU7WSIBLGCEHXGIEKJCQPW3RGZOOU4WA4QFUVU3J",
                "selling_asset_type": "credit_alphanum12",
                "source_account": "GDVRZI2IQUWCCOMIAWGZA4DLZNYYS7TAD2G2EHYFSGP3LVOVRCJLOBBJ",
                "transaction_hash": "0a33e149a21b67e11fabb30e41adb08984766550f0e83bd2ae66b33a183dd452",
                "transaction_successful": true,
                "type": "manage_sell_offer",
                "type_i": 3
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/ledgers/45678721/operations?cursor=196188612818112514&limit=2&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/ledgers/45678721/operations?cursor=196188612818112513&limit=2&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/ledgers/45678721/operations?cursor=&limit=2&order=asc"
        }
    }
}
```

