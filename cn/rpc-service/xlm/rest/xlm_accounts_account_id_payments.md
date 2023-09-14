---
title: xlm:/accounts/{account_id}/payments \[GET\]
description: This endpoint represents successful payments for a given account and canbe used in streaming mode. Streaming mode allows you to listen for newpayments for this account as they are added to the Stellar ledger. Ifcalled in streaming mode, Horizon will start at the earliest knownpayment unless a cursor is set, in which case it will start from thatcursor. By setting the cursor value to now, you can stream paymentscreated since your request time.
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
curl --location --request GET 'https://xlm.getblock.io/mainnet/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/payments?limit=2' 
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
                        "href": "https://xlm.getblock.io/operations/196256365927284737/effects"
                    },
                    "precedes": {
                        "href": "https://xlm.getblock.io/effects?order=asc&cursor=196256365927284737"
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/operations/196256365927284737"
                    },
                    "succeeds": {
                        "href": "https://xlm.getblock.io/effects?order=desc&cursor=196256365927284737"
                    },
                    "transaction": {
                        "href": "https://xlm.getblock.io/transactions/46e5a6864c2b0f503bab288973582b3fd1e300834f4d3b122f1ff700c34af138"
                    }
                },
                "amount": "136.2779760",
                "asset_code": "GBPV",
                "asset_issuer": "GDB6ZOJ46MDSERVTH2B7P6C4LEAWU3UDJZLPUFERROEDV774U4AQIG5G",
                "asset_type": "credit_alphanum4",
                "created_at": "2023-04-05T11:22:42Z",
                "from": "GAXC2HGINK6V36EO7UI7SI4OK5KGS4QKUDPUFRYASWKW6AHKAIDSS4YW",
                "id": "196256365927284737",
                "paging_token": "196256365927284737",
                "source_account": "GAXC2HGINK6V36EO7UI7SI4OK5KGS4QKUDPUFRYASWKW6AHKAIDSS4YW",
                "to": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
                "transaction_hash": "46e5a6864c2b0f503bab288973582b3fd1e300834f4d3b122f1ff700c34af138",
                "transaction_successful": true,
                "type": "payment",
                "type_i": 1
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/payments?cursor=196256872733466625&limit=5&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/payments?cursor=196256365927284737&limit=5&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/payments?cursor=&limit=5&order=asc"
        }
    }
}
```

