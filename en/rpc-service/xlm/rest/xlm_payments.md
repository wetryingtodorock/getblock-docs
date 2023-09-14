---
title: xlm:/payments \[GET\]
description: This endpoint lists all Successful payment-related operations and can beused in streaming mode. Streaming mode allows you to listen for newpayments as they are added to the Stellar ledger. If called in streamingmode, Horizon will start at the earliest known payment unless a cursoris set, in which case it will start from that cursor. By setting thecursor value to now, you can stream payments created since your requesttime. Operations that can be returned by this endpoint includecreate_account, payment, path_payment_strict_recieve,path_payment_strict_send, and account_merge .
---

### Parameters


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
curl --location --request GET 'https://xlm.getblock.io/mainnet/payments?limit=1' 
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
                        "href": "https://xlm.getblock.io/operations/196188608523247619/effects"
                    },
                    "precedes": {
                        "href": "https://xlm.getblock.io/effects?order=asc&cursor=196188608523247619"
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/operations/196188608523247619"
                    },
                    "succeeds": {
                        "href": "https://xlm.getblock.io/effects?order=desc&cursor=196188608523247619"
                    },
                    "transaction": {
                        "href": "https://xlm.getblock.io/transactions/b99c9cf36e5848938b50c921d1203200b6a90379f10564685c14a81e54a07962"
                    }
                },
                "amount": "1706.8540213",
                "asset_code": "XXA",
                "asset_issuer": "GC4HS4CQCZULIOTGLLPGRAAMSBDLFRR6Y7HCUQG66LNQDISXKIXXADIM",
                "asset_type": "credit_alphanum4",
                "created_at": "2023-04-04T10:14:50Z",
                "from": "GDVHBUCHE6LS7O4R2366YDLL2LLSAIH4I6YCX3EK2KZLBOV7H6QA7GUX",
                "id": "196188608523247619",
                "paging_token": "196188608523247619",
                "source_account": "GDVHBUCHE6LS7O4R2366YDLL2LLSAIH4I6YCX3EK2KZLBOV7H6QA7GUX",
                "to": "GDTEGWSEHTJTKN4CRDZNW3ZJZQLFRVMRMQ7M6BUDZLB54XXQMMI2XRUF",
                "transaction_hash": "b99c9cf36e5848938b50c921d1203200b6a90379f10564685c14a81e54a07962",
                "transaction_successful": true,
                "type": "payment",
                "type_i": 1
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/payments?cursor=196188608523247620&limit=2&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/payments?cursor=196188608523247619&limit=2&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/payments?cursor=&limit=2&order=asc"
        }
    }
}
```

