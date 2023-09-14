---
title: xlm:/operations/{operation_id}/effects \[GET\]
description: This endpoint returns the effects of a specific operation.
---

### Parameters


`id` - path

string, required

The ID number for this operation.

`cursor` - query

integer, optional

A number that points to a specific location in a collection of responses
and is pulled from the paging_token value of a record.

`order` - query

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
curl --location --request GET 'https://xlm.getblock.io/mainnet/operations/196188608523145217/effects?limit=2' 
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
                        "href": "https://horizon.stellar.org/operations/196188608523145217"
                    },
                    "succeeds": {
                        "href": "https://horizon.stellar.org/effects?order=desc&cursor=196188608523145217-1"
                    },
                    "precedes": {
                        "href": "https://horizon.stellar.org/effects?order=asc&cursor=196188608523145217-1"
                    }
                },
                "id": "0196188608523145217-0000000001",
                "paging_token": "196188608523145217-1",
                "account": "GALSPNVKGNRJ3VIOQ26QKPZBDCTVJK7XPLSPF3UVZV3JJXCKVCHNSPCK",
                "type": "account_credited",
                "type_i": 2,
                "created_at": "2020-02-21T20:27:30Z",
                "asset_type": "credit_alphanum4",
                "asset_code": "NODL",
                "asset_issuer": "GB2Y3AWXVROM2BHFQKQPTWKIOI3TZEBBD3LTKTVQTKEPXGOBE742NODL",
                "amount": "0.0000027"
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/operations/196188608523145217/effects?cursor=&limit=2&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/operations/196188608523145217/effects?cursor=&limit=2&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/operations/196188608523145217/effects?cursor=&limit=2&order=asc"
        }
    }
}
```

