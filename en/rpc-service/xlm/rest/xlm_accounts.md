---
title: xlm:/accounts \[GET\]
description: This endpoint lists accounts by one of four filters  signer, asset,liquidity pool or sponsor.
---

### Parameters


`sponser` - query

string, optional

Account ID of the sponsor. Every account in the response will either be
sponsored by the given account ID or have a subentry (trustline, offer,
or data entry) which is sponsored by the given account ID.

`asset` - query

any

An issued asset represented as “Code:IssuerAccountID”. Every account in
the response will have a trustline for the given asset.

`signer` - query

string, optional

Account ID of the signer. Every account in the response will have the
given account ID as a signer.

`liquidy_pool` - query

any, optional

With this parameter, the results will include only accounts which have
trustlines to the specified liquidity pool.

`cursor` - query

integer, optional

A number that points to a specific location in a collection of responses
and is pulled from the paging_token value of a record.

`order` - query

Possible values: \[asc, desc\], optional

A designation of the order in which records should appear. Options
include asc (ascending) or desc (descending). If this argument is not
set, it defaults to asc.

`limit` - query

integer, optional

The maximum number of records returned. The limit can range from 1 to
200 - an upper limit that is hardcoded in Horizon for performance
reasons. If this argument is not designated, it defaults to 10.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/accounts?signer=GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ&limit=2' 
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
                    "data": {
                        "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/data/{key}",
                        "templated": true
                    },
                    "effects": {
                        "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/effects{?cursor,limit,order}",
                        "templated": true
                    },
                    "offers": {
                        "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/offers{?cursor,limit,order}",
                        "templated": true
                    },
                    "operations": {
                        "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/operations{?cursor,limit,order}",
                        "templated": true
                    },
                    "payments": {
                        "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/payments{?cursor,limit,order}",
                        "templated": true
                    },
                    "self": {
                        "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ"
                    },
                    "trades": {
                        "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/trades{?cursor,limit,order}",
                        "templated": true
                    },
                    "transactions": {
                        "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/transactions{?cursor,limit,order}",
                        "templated": true
                    }
                },
                "account_id": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
                "balances": [
                    {
                        "asset_code": "GBPV",
                        "asset_issuer": "GDB6ZOJ46MDSERVTH2B7P6C4LEAWU3UDJZLPUFERROEDV774U4AQIG5G",
                        "asset_type": "credit_alphanum4",
                        "balance": "75521.3750022",
                        "buying_liabilities": "20292.5295000",
                        "is_authorized": true,
                        "is_authorized_to_maintain_liabilities": true,
                        "last_modified_ledger": 46844540,
                        "limit": "922337203685.4775807",
                        "selling_liabilities": "29432.0000000"
                    }
                ],
                "data": {},
                "flags": {
                    "auth_clawback_enabled": false,
                    "auth_immutable": false,
                    "auth_required": false,
                    "auth_revocable": false
                },
                "home_domain": "lobstr.co",
                "id": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
                "inflation_destination": "GDCHDRSDOBRMSUDKRE2C4U4KDLNEATJPIHHR2ORFL5BSD56G4DQXL4VW",
                "last_modified_ledger": 46844540,
                "last_modified_time": "2023-06-20T19:46:04Z",
                "num_sponsored": 0,
                "num_sponsoring": 0,
                "paging_token": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
                "sequence": "185387470148735007",
                "sequence_ledger": 46844540,
                "sequence_time": "1687290364",
                "signers": [
                    {
                        "key": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
                        "type": "ed25519_public_key",
                        "weight": 1
                    }
                ],
                "subentry_count": 15,
                "thresholds": {
                    "high_threshold": 0,
                    "low_threshold": 0,
                    "med_threshold": 0
                }
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/accounts?cursor=GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ&limit=2&order=asc&signer=GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ"
        },
        "prev": {
            "href": "https://xlm.getblock.io/accounts?cursor=GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ&limit=2&order=desc&signer=GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ"
        },
        "self": {
            "href": "https://xlm.getblock.io/accounts?cursor=&limit=2&order=asc&signer=GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ"
        }
    }
}
```

