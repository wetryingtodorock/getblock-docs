---
title: xlm:/effects \[GET\]
description: This endpoint lists all effects and can be used in streaming mode.Streaming mode allows you to listen for new effects as they are added tothe Stellar ledger. If called in streaming mode, Horizon will start atthe earliest known effect unless a cursor is set, in which case it willstart from that cursor. By setting the cursor value to now, you canstream effects created since your request time.
---

### Parameters


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

limit, optional

The maximum number of records returned. The limit can range from 1 to
200 - an upper limit that is hardcoded in Horizon for performance
reasons. If this argument isn't designated, it defaults to 10.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/effects?cursor=196188608523149313&limit=1' 
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
                        "href": "https://xlm.getblock.io/operations/196188608523157505"
                    },
                    "precedes": {
                        "href": "https://xlm.getblock.io/effects?order=asc&cursor=196188608523157505-2"
                    },
                    "succeeds": {
                        "href": "https://xlm.getblock.io/effects?order=desc&cursor=196188608523157505-2"
                    }
                },
                "account": "GDXID5C7CB3HRT7OHPNTYO2A53UUQB7EPKTZAMV3HTOPKE5JYJFT2P7P",
                "bought_amount": "395.0000000",
                "bought_asset_code": "EURV",
                "bought_asset_issuer": "GDB6ZOJ46MDSERVTH2B7P6C4LEAWU3UDJZLPUFERROEDV774U4AQIG5G",
                "bought_asset_type": "credit_alphanum4",
                "created_at": "2023-04-04T10:14:50Z",
                "id": "0196188608523157505-0000000002",
                "offer_id": "1230882975",
                "paging_token": "196188608523157505-2",
                "seller": "GAOOWVWIXY5XSVWVVRZX2G4LCDHX6HPKUAVH7UZY5DFWB3KOWRURARZS",
                "sold_amount": "431.5375036",
                "sold_asset_code": "USDV",
                "sold_asset_issuer": "GDB6ZOJ46MDSERVTH2B7P6C4LEAWU3UDJZLPUFERROEDV774U4AQIG5G",
                "sold_asset_type": "credit_alphanum4",
                "type": "trade",
                "type_i": 33
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/effects?cursor=196188608523231233-1&limit=5&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/effects?cursor=196188608523157505-1&limit=5&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/effects?cursor=196188608523149313&limit=5&order=asc"
        }
    }
}
```

