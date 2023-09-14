---
title: xlm:/assets \[GET\]
description: This endpoint lists all assets.
---

### Parameters


`asset_code` - query

any, optional

The code of the asset you would like to filter by.

`asset_issuer` - query

any, optional

The Stellar address of the issuer for the asset you would like to filter
by.

`cursor` - query

integer, optional

A number that points to a specific location in a collection of responses
and is pulled from the paging_token value of a record.

`order` - query

Possible values: \[asc, desc\], optional

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
curl --location --request GET 'https://xlm.getblock.io/mainnet//assets?asset_issuer=GBBJZOYEGLOCW32Q4ZGWRWQ7UKIGMMIQXIRBBBOVJVFJTZW7CR2VQKAT&order=asc&limit=2&' 
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
                    "toml": {
                        "href": "https://emily.stellarskull.io/.well-known/stellar.toml"
                    }
                },
                "accounts": {
                    "authorized": 25,
                    "authorized_to_maintain_liabilities": 0,
                    "unauthorized": 0
                },
                "amount": "1000.0000000",
                "asset_code": "0",
                "asset_issuer": "GBBJZOYEGLOCW32Q4ZGWRWQ7UKIGMMIQXIRBBBOVJVFJTZW7CR2VQKAT",
                "asset_type": "credit_alphanum4",
                "balances": {
                    "authorized": "1000.0000000",
                    "authorized_to_maintain_liabilities": "0.0000000",
                    "unauthorized": "0.0000000"
                },
                "claimable_balances_amount": "0.0000000",
                "flags": {
                    "auth_clawback_enabled": false,
                    "auth_immutable": false,
                    "auth_required": false,
                    "auth_revocable": false
                },
                "liquidity_pools_amount": "0.0000000",
                "num_accounts": 25,
                "num_claimable_balances": 0,
                "num_liquidity_pools": 0,
                "paging_token": "0_GBBJZOYEGLOCW32Q4ZGWRWQ7UKIGMMIQXIRBBBOVJVFJTZW7CR2VQKAT_credit_alphanum4"
            },
            {
                "_links": {
                    "toml": {
                        "href": "https://emily.stellarskull.io/.well-known/stellar.toml"
                    }
                },
                "accounts": {
                    "authorized": 92,
                    "authorized_to_maintain_liabilities": 0,
                    "unauthorized": 0
                },
                "amount": "999.9600000",
                "asset_code": "1",
                "asset_issuer": "GBBJZOYEGLOCW32Q4ZGWRWQ7UKIGMMIQXIRBBBOVJVFJTZW7CR2VQKAT",
                "asset_type": "credit_alphanum4",
                "balances": {
                    "authorized": "999.9600000",
                    "authorized_to_maintain_liabilities": "0.0000000",
                    "unauthorized": "0.0000000"
                },
                "claimable_balances_amount": "0.0000000",
                "flags": {
                    "auth_clawback_enabled": false,
                    "auth_immutable": false,
                    "auth_required": false,
                    "auth_revocable": false
                },
                "liquidity_pools_amount": "0.0000000",
                "num_accounts": 92,
                "num_claimable_balances": 0,
                "num_liquidity_pools": 0,
                "paging_token": "1_GBBJZOYEGLOCW32Q4ZGWRWQ7UKIGMMIQXIRBBBOVJVFJTZW7CR2VQKAT_credit_alphanum4"
            }
        ]
    },
    "_links": {
        "next": {
            "href": "https://xlm.getblock.io/assets?asset_issuer=GBBJZOYEGLOCW32Q4ZGWRWQ7UKIGMMIQXIRBBBOVJVFJTZW7CR2VQKAT&cursor=1_GBBJZOYEGLOCW32Q4ZGWRWQ7UKIGMMIQXIRBBBOVJVFJTZW7CR2VQKAT_credit_alphanum4&limit=2&order=asc"
        },
        "prev": {
            "href": "https://xlm.getblock.io/assets?asset_issuer=GBBJZOYEGLOCW32Q4ZGWRWQ7UKIGMMIQXIRBBBOVJVFJTZW7CR2VQKAT&cursor=0_GBBJZOYEGLOCW32Q4ZGWRWQ7UKIGMMIQXIRBBBOVJVFJTZW7CR2VQKAT_credit_alphanum4&limit=2&order=desc"
        },
        "self": {
            "href": "https://xlm.getblock.io/assets?asset_issuer=GBBJZOYEGLOCW32Q4ZGWRWQ7UKIGMMIQXIRBBBOVJVFJTZW7CR2VQKAT&cursor=&limit=2&order=asc"
        }
    }
}
```

