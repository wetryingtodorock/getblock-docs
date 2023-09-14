---
title: xlm:/accounts/{account_id}/effects \[GET\]
description: This endpoint returns the effects of a specific account and can be usedin streaming mode. Streaming mode allows you to listen for new effectsfor this account as they are added to the Stellar ledger. If called instreaming mode, Horizon will start at the earliest known effect unless acursor is set, in which case it will start from that cursor. By settingthe cursor value to now, you can stream effects created since yourrequest time.
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
curl --location --request GET 'https://xlm.getblock.io/mainnet/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/effects?limit=5' 
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
                        "href": "https://xlm.getblock.io/operations/196188608523149313"
                    },
                    "precedes": {
                        "href": "https://xlm.getblock.io/effects?order=asc&cursor=196188608523149313-2"
                    },
                    "succeeds": {
                        "href": "https://xlm.getblock.io/effects?order=desc&cursor=196188608523149313-2"
                    }
                },
                "account": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
                "bought_amount": "166.2500000",
                "bought_asset_code": "USDV",
                "bought_asset_issuer": "GDB6ZOJ46MDSERVTH2B7P6C4LEAWU3UDJZLPUFERROEDV774U4AQIG5G",
                "bought_asset_type": "credit_alphanum4",
                "created_at": "2023-04-04T10:14:50Z",
                "id": "0196188608523149313-0000000002",
                "offer_id": "1230905851",
                "paging_token": "196188608523149313-2",
                "seller": "GBUO63ZYZUGNJ6Z3OG2WQAYGVOPUD72REX6FKSAN3YOMUR3OYAPVYOPU",
                "sold_amount": "133.0000000",
                "sold_asset_code": "GBPV",
                "sold_asset_issuer": "GDB6ZOJ46MDSERVTH2B7P6C4LEAWU3UDJZLPUFERROEDV774U4AQIG5G",
                "sold_asset_type": "credit_alphanum4",
                "type": "trade",
                "type_i": 33
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/effects?cursor=196188621408133121-2&limit=5&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/effects?cursor=196188608523149313-2&limit=5&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/effects?cursor=&limit=5&order=asc"
        }
    }
}
```

