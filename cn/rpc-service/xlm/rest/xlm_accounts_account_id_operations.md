---
title: xlm:/accounts/{account_id}/operations \[GET\]
description: This endpoint represents successful operations for a given account andcan be used in streaming mode. Streaming mode allows you to listen fornew operations for this account as they are added to the Stellar ledger.If called in streaming mode, Horizon will start at the earliest knownoperation unless a cursor is set, in which case it will start from thatcursor. By setting the cursor value to now, you can stream operationscreated since your request time.
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
curl --location --request GET 'https://xlm.getblock.io/mainnet/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/operations?limit=2' 
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
                        "href": "https://xlm.getblock.io/operations/196188621408321537/effects"
                    },
                    "precedes": {
                        "href": "https://xlm.getblock.io/effects?order=asc&cursor=196188621408321537"
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/operations/196188621408321537"
                    },
                    "succeeds": {
                        "href": "https://xlm.getblock.io/effects?order=desc&cursor=196188621408321537"
                    },
                    "transaction": {
                        "href": "https://xlm.getblock.io/transactions/754b492c09963177def246f02e66452b6c9bf2532cb1b00cd5691d34ae408747"
                    }
                },
                "amount": "0.0000000",
                "buying_asset_code": "GBPV",
                "buying_asset_issuer": "GDB6ZOJ46MDSERVTH2B7P6C4LEAWU3UDJZLPUFERROEDV774U4AQIG5G",
                "buying_asset_type": "credit_alphanum4",
                "created_at": "2023-04-04T10:15:07Z",
                "id": "196188621408321537",
                "offer_id": "1230905759",
                "paging_token": "196188621408321537",
                "price": "0.8012821",
                "price_r": {
                    "d": 10000000,
                    "n": 8012821
                },
                "selling_asset_code": "USDV",
                "selling_asset_issuer": "GDB6ZOJ46MDSERVTH2B7P6C4LEAWU3UDJZLPUFERROEDV774U4AQIG5G",
                "selling_asset_type": "credit_alphanum4",
                "source_account": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
                "transaction_hash": "754b492c09963177def246f02e66452b6c9bf2532cb1b00cd5691d34ae408747",
                "transaction_successful": true,
                "type": "manage_sell_offer",
                "type_i": 3
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/operations?cursor=196188754552455169&limit=5&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/operations?cursor=196188621408321537&limit=5&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/operations?cursor=&limit=5&order=asc"
        }
    }
}
```

