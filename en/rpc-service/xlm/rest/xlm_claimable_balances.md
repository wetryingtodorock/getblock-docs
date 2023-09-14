---
title: xlm:/claimable_balances \[GET\]
description: This endpoint lists all available claimable balances.
---

### Parameters


`sponser` - query

string, optional

Account ID of the sponsor. Every account in the response will either be
sponsored by the given account ID or have a subentry (trustline, offer,
or data entry) which is sponsored by the given account ID.

`asset` - query

any, optional

An issued asset represented as “Code:IssuerAccountID”. Every account in
the response will have a trustline for the given asset.

`claimant` - query

any, optional

Account ID of the destination address. Only include claimable balances
which can be claimed by the given account ID.

`cursor` - query

integer, optional

A number that points to a specific location in a collection of responses
and is pulled from the paging_token value of a record.

`order` - query

optional. possible options are 'asc' and 'desc'

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
curl --location --request GET 'https://xlm.getblock.io/mainnet/claimable_balances?sponser=GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ&limit=2' 
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
                    "operations": {
                        "href": "https://xlm.getblock.io/claimable_balances/00000000178826fbfe339e1f5c53417c6fedfe2c05e8bec14303143ec46b38981b09c3f9/operations{?cursor,limit,order}",
                        "templated": true
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/claimable_balances/00000000178826fbfe339e1f5c53417c6fedfe2c05e8bec14303143ec46b38981b09c3f9"
                    },
                    "transactions": {
                        "href": "https://xlm.getblock.io/claimable_balances/00000000178826fbfe339e1f5c53417c6fedfe2c05e8bec14303143ec46b38981b09c3f9/transactions{?cursor,limit,order}",
                        "templated": true
                    }
                },
                "amount": "0.1000000",
                "asset": "BODHI:GDCJIHD3623OCYNH65UUQC3NLG2D6YCNCDPZULRLCLOA76TBQRL6A3TF",
                "claimants": [
                    {
                        "destination": "GBEUDKANIFPTFHPWJ5T3R6RIO36RQBFGHYPAQ6STH7KMNDHAT36LHOLD",
                        "predicate": {
                            "unconditional": true
                        }
                    }
                ],
                "flags": {
                    "clawback_enabled": false
                },
                "id": "00000000178826fbfe339e1f5c53417c6fedfe2c05e8bec14303143ec46b38981b09c3f9",
                "last_modified_ledger": 32747318,
                "last_modified_time": null,
                "paging_token": "32747318-00000000178826fbfe339e1f5c53417c6fedfe2c05e8bec14303143ec46b38981b09c3f9",
                "sponsor": "GDCJIHD3623OCYNH65UUQC3NLG2D6YCNCDPZULRLCLOA76TBQRL6A3TF"
            },
            {
                "_links": {
                    "operations": {
                        "href": "https://xlm.getblock.io/claimable_balances/00000000446bbc79c503c759275d433b088a89b122981ff104a76bc4fdb8e212a87eae35/operations{?cursor,limit,order}",
                        "templated": true
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/claimable_balances/00000000446bbc79c503c759275d433b088a89b122981ff104a76bc4fdb8e212a87eae35"
                    },
                    "transactions": {
                        "href": "https://xlm.getblock.io/claimable_balances/00000000446bbc79c503c759275d433b088a89b122981ff104a76bc4fdb8e212a87eae35/transactions{?cursor,limit,order}",
                        "templated": true
                    }
                },
                "amount": "11.0000000",
                "asset": "BUG:GC75UHF5DYWGR5T2AZVAGI7VPVSMUAW6ACJ3BXG3ZVXJQEJA5VBU6BUG",
                "claimants": [
                    {
                        "destination": "GBRJH345POLYMR2CPIU4EPQSAKSX76L4NCP3W2E7MGT367LNKF3DK56K",
                        "predicate": {
                            "unconditional": true
                        }
                    }
                ],
                "flags": {
                    "clawback_enabled": false
                },
                "id": "00000000446bbc79c503c759275d433b088a89b122981ff104a76bc4fdb8e212a87eae35",
                "last_modified_ledger": 32862748,
                "last_modified_time": null,
                "paging_token": "32862748-00000000446bbc79c503c759275d433b088a89b122981ff104a76bc4fdb8e212a87eae35",
                "sponsor": "GBGR33CE23GH4XMXHAAYFLOKD353KAHDO3PYFLNC5TEZQB7L6LESD2M5"
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/claimable_balances?cursor=32862748-00000000446bbc79c503c759275d433b088a89b122981ff104a76bc4fdb8e212a87eae35&limit=2&order=asc&sponser=GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ"
        },
        "prev": {
            "href": "https://xlm.getblock.io/claimable_balances?cursor=32747318-00000000178826fbfe339e1f5c53417c6fedfe2c05e8bec14303143ec46b38981b09c3f9&limit=2&order=desc&sponser=GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ"
        },
        "self": {
            "href": "https://xlm.getblock.io/claimable_balances?cursor=&limit=2&order=asc&sponser=GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ"
        }
    }
}
```

