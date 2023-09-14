---
title: xlm:/offers/{offer_id}/trades \[GET\]
description: This endpoint represents all trades for a given offer and can be used instreaming mode. Streaming mode allows you to listen for trades for thisoffer as they are added to the Stellar ledger. If called in streamingmode, Horizon will start at the earliest known trade unless a cursor isset, in which case it will start from that cursor. By setting the cursorvalue to now, you can stream trades created since your request time.
---

### Parameters


`offer_id` - path

any, required

A unique identifier for this offer.

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
curl --location --request GET 'https://xlm.getblock.io/mainnet/offers/167/trades' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_embedded": {
        "records": []
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/offers/167/trades?cursor=&limit=10&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/offers/167/trades?cursor=&limit=10&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/offers/167/trades?cursor=&limit=10&order=asc"
        }
    }
}
```

