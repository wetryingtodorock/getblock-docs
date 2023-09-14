---
title: xlm:/ledgers/{sequence}/effects \[GET\]
description: This endpoint returns the effects of a specific ledger.
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

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/ledgers/45678721/effects?limit=1' 
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
                        "href": "https://xlm.getblock.io/operations/196188612818120705"
                    },
                    "precedes": {
                        "href": "https://xlm.getblock.io/effects?order=asc&cursor=196188612818120705-1"
                    },
                    "succeeds": {
                        "href": "https://xlm.getblock.io/effects?order=desc&cursor=196188612818120705-1"
                    }
                },
                "account": "GADWJDKBOXNDBQJ5VQX2SB576K6MC6DEBRCY63GGR6OSUTYSVRQITQNT",
                "auth_required_flag": true,
                "created_at": "2023-04-04T10:14:56Z",
                "id": "0196188612818120705-0000000001",
                "paging_token": "196188612818120705-1",
                "type": "account_flags_updated",
                "type_i": 6
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/ledgers/45678721/effects?cursor=196188612818120706-1&limit=2&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/ledgers/45678721/effects?cursor=196188612818120705-1&limit=2&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/ledgers/45678721/effects?cursor=&limit=2&order=asc"
        }
    }
}
```

