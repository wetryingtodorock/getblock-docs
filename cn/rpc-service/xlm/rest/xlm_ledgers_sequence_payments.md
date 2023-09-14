---
title: xlm:/ledgers/{sequence}/payments \[GET\]
description: This endpoint returns successful operations in a specific ledger.
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
curl --location --request GET 'https://xlm.getblock.io/mainnet/ledgers/45678721/payments?limit=1' 
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
                        "href": "https://xlm.getblock.io/operations/196188612818243585/effects"
                    },
                    "precedes": {
                        "href": "https://xlm.getblock.io/effects?order=asc&cursor=196188612818243585"
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/operations/196188612818243585"
                    },
                    "succeeds": {
                        "href": "https://xlm.getblock.io/effects?order=desc&cursor=196188612818243585"
                    },
                    "transaction": {
                        "href": "https://xlm.getblock.io/transactions/a22ba0784d86507c3ba0757de3ae483e1b6fc52015c1f05d0ec1e1fb46dce676"
                    }
                },
                "amount": "329.6102741",
                "asset_code": "AQUA",
                "asset_issuer": "GBNZILSTVQZ4R7IKQDGHYGY2QXL5QOFJYQMXPKWRRM5PAV7Y4M67AQUA",
                "asset_type": "credit_alphanum4",
                "created_at": "2023-04-04T10:14:56Z",
                "from": "GC5VEAWX7C3GSTW7RUKJKMQWXYZFW5TH4NGI4ZQSF6LNLUYSDGBVANBA",
                "id": "196188612818243585",
                "paging_token": "196188612818243585",
                "source_account": "GC5VEAWX7C3GSTW7RUKJKMQWXYZFW5TH4NGI4ZQSF6LNLUYSDGBVANBA",
                "to": "GBHMVD6KDFUMCS5HDHGP2TMY5FQN53BPJNUOWXVK2BENSH2ZZ3UZ4LIQ",
                "transaction_hash": "a22ba0784d86507c3ba0757de3ae483e1b6fc52015c1f05d0ec1e1fb46dce676",
                "transaction_successful": true,
                "type": "payment",
                "type_i": 1
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/ledgers/45678721/payments?cursor=196188612818243585&limit=2&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/ledgers/45678721/payments?cursor=196188612818219009&limit=2&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/ledgers/45678721/payments?cursor=&limit=2&order=asc"
        }
    }
}
```

