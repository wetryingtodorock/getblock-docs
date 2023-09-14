---
title: xlm:/transactions/{transaction_hash}/effects \[GET\]
description: This endpoint returns the effects of a specific transaction.
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

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet//transactions/512a9946bc7ff4a363299f14f79e0beb9b9cdbd0103e3a69a44446a0aa6471a8/effects?limit=1' 
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
                    "operation": {
                        "href": "https://horizon.stellar.org/operations/121628667754319873"
                    },
                    "succeeds": {
                        "href": "https://horizon.stellar.org/effects?order=desc&cursor=121628667754319873-1"
                    },
                    "precedes": {
                        "href": "https://horizon.stellar.org/effects?order=asc&cursor=121628667754319873-1"
                    }
                },
                "id": "0121628667754319873-0000000001",
                "paging_token": "121628667754319873-1",
                "account": "GAHK7EEG2WWHVKDNT4CEQFZGKF2LGDSW2IVM4S5DP42RBW3K6BTODB4A",
                "type": "account_credited",
                "type_i": 2,
                "created_at": "2020-02-20T21:18:33Z",
                "asset_type": "native",
                "amount": "1573.5112616"
            },
            {
                "_links": {
                    "operation": {
                        "href": "https://horizon.stellar.org/operations/121628667754319873"
                    },
                    "succeeds": {
                        "href": "https://horizon.stellar.org/effects?order=desc&cursor=121628667754319873-2"
                    },
                    "precedes": {
                        "href": "https://horizon.stellar.org/effects?order=asc&cursor=121628667754319873-2"
                    }
                },
                "id": "0121628667754319873-0000000002",
                "paging_token": "121628667754319873-2",
                "account": "GA2XP4KMY4KWNPW4KUCUKYUF2J7Y6HO5HLPUEA3VPVSMYCM3TGNEZP5S",
                "type": "account_debited",
                "type_i": 3,
                "created_at": "2020-02-20T21:18:33Z",
                "asset_type": "native",
                "amount": "1573.5112616"
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/transactions/512a9946bc7ff4a363299f14f79e0beb9b9cdbd0103e3a69a44446a0aa6471a8/effects?cursor=&limit=2&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/transactions/512a9946bc7ff4a363299f14f79e0beb9b9cdbd0103e3a69a44446a0aa6471a8/effects?cursor=&limit=2&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/transactions/512a9946bc7ff4a363299f14f79e0beb9b9cdbd0103e3a69a44446a0aa6471a8/effects?cursor=&limit=2&order=asc"
        }
    }
}
```

