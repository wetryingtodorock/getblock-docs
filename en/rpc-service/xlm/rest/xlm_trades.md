---
title: xlm:/trades \[GET\]
description: This endpoint lists all trades and can be used in streaming mode.Streaming mode allows you to listen for new trades as they are added tothe Stellar ledger. If called in streaming mode, Horizon will start atthe earliest known trade unless a cursor is set, in which case it willstart from that cursor. By setting the cursor value to now, you canstream trades created since your request time. When filtering for aspecific orderbook, you must use use all six of these argumentsbase_asset_type, base_asset_issuer, base_asset_code, counter_asset_type,counter_asset_issuer, and counter_asset_code. If the base or counterasset is XLM, you only need to indicate the asset type as native and donot need to designate the code or the issuer.
---

### Parameters


`offer_id` - query

any, optional

The offer ID. Used to filter for trades originating from a specific
offer.

`base_asset_type` - query

string, optional

The type for the base asset. Either native, credit_alphanum4, or
credit_alphanum12.

`base_asset_issuer` - query

string, optional

The Stellar address of the base asset’s issuer.

`base_asset_code` - query

string, optional

The code for the base asset.

`counter_asset_type` - query

string, optional

The type for the counter asset. Either native, credit_alphanum4, or
credit_alphanum12.

`counter_asset_issuer` - query

string, optional

The Stellar address of the counter asset’s issuer.

`counter_asset_code` - query

any, optional

The code for the counter asset.

`trade_type` - query

string, optional

Can be set to all, orderbook, or liquidity_pools to filter only trades
executed across a given mechanism.

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
curl --location --request GET 'https://xlm.getblock.io/mainnet/trades?limit=1' 
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
                    "base": {
                        "href": "https://xlm.getblock.io/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ"
                    },
                    "counter": {
                        "href": "https://xlm.getblock.io/accounts/GAHGDBLK4OOCP2JTCTDQR2HBT7SZ47ICD5T3HDKVWN4C4CBEIDBYJT33"
                    },
                    "operation": {
                        "href": "https://xlm.getblock.io/operations/196188608523186177"
                    },
                    "self": {
                        "href": ""
                    }
                },
                "base_account": "GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ",
                "base_amount": "378.0000000",
                "base_asset_code": "GBPV",
                "base_asset_issuer": "GDB6ZOJ46MDSERVTH2B7P6C4LEAWU3UDJZLPUFERROEDV774U4AQIG5G",
                "base_asset_type": "credit_alphanum4",
                "base_is_seller": true,
                "base_offer_id": "1230903109",
                "counter_account": "GAHGDBLK4OOCP2JTCTDQR2HBT7SZ47ICD5T3HDKVWN4C4CBEIDBYJT33",
                "counter_amount": "472.6890000",
                "counter_asset_code": "USDV",
                "counter_asset_issuer": "GDB6ZOJ46MDSERVTH2B7P6C4LEAWU3UDJZLPUFERROEDV774U4AQIG5G",
                "counter_asset_type": "credit_alphanum4",
                "counter_offer_id": "4807874626950574081",
                "id": "196188608523186177-0",
                "ledger_close_time": "2023-04-04T10:14:50Z",
                "paging_token": "196188608523186177-0",
                "price": {
                    "d": "2000",
                    "n": "2501"
                },
                "trade_type": "orderbook"
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/trades?cursor=196188608523235334-0&limit=10&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/trades?cursor=196188608523149313-0&limit=10&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/trades?cursor=&limit=10&order=asc"
        }
    }
}
```

