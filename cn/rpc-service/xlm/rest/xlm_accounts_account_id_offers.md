---
title: xlm:/accounts/{account_id}/offers \[GET\]
description: This endpoint represents all offers a given account has currently openand can be used in streaming mode. Streaming mode allows you to listenfor new offers for this account as they are added to the Stellar ledger.If called in streaming mode, Horizon will start at the earliest knownoffer unless a cursor is set, in which case it will start from thatcursor. By setting the cursor value to now, you can stream offerscreated since your request time.
---

### Parameters


`account_id` - path

string, required

This account's public key encoded in a base32 string representation.

`cursor` - query

integer, optional

A number that points to a specific location in a collection of responses
and is pulled from the paging_token value of a record.

`order` - query

Possible values: \[asc, desc\], optional

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
curl --location --request GET 'https://xlm.getblock.io/mainnet/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/offers' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_links": {
        "self": {
            "href": "https://horizon.stellar.org/accounts/GD3CJYUTZAY6JQF4CEI6Z7VW5O6VNGKZTBYUECTOJPEDTB7I2HZSPI2K/offers?cursor=&limit=10&order=asc"
        },
        "next": {
            "href": "https://horizon.stellar.org/accounts/GD3CJYUTZAY6JQF4CEI6Z7VW5O6VNGKZTBYUECTOJPEDTB7I2HZSPI2K/offers?cursor=164943216&limit=10&order=asc"
        },
        "prev": {
            "href": "https://horizon.stellar.org/accounts/GD3CJYUTZAY6JQF4CEI6Z7VW5O6VNGKZTBYUECTOJPEDTB7I2HZSPI2K/offers?cursor=164555927&limit=10&order=desc"
        }
    },
    "_embedded": {
        "records": [
            {
                "_links": {
                    "self": {
                        "href": "https://horizon.stellar.org/offers/164555927"
                    },
                    "offer_maker": {
                        "href": "https://horizon.stellar.org/accounts/GD3CJYUTZAY6JQF4CEI6Z7VW5O6VNGKZTBYUECTOJPEDTB7I2HZSPI2K"
                    }
                },
                "id": 164555927,
                "paging_token": "164555927",
                "seller": "GD3CJYUTZAY6JQF4CEI6Z7VW5O6VNGKZTBYUECTOJPEDTB7I2HZSPI2K",
                "selling": {
                    "asset_type": "native"
                },
                "buying": {
                    "asset_type": "credit_alphanum4",
                    "asset_code": "BB1",
                    "asset_issuer": "GD5J6HLF5666X4AZLTFTXLY46J5SW7EXRKBLEYPJP33S33MXZGV6CWFN"
                },
                "amount": "214.9999939",
                "price_r": {
                    "n": 10000000,
                    "d": 86000001
                },
                "price": "0.1162791",
                "last_modified_ledger": 28383147,
                "last_modified_time": "2020-02-24T22:58:38Z"
            }
        ]
    }
}
```

