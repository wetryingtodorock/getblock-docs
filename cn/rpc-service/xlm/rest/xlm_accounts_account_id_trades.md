---
title: xlm:/accounts/{account_id}/trades \[GET\]
description: This endpoint represents all trades for a given account and can be usedin streaming mode. Streaming mode allows you to listen for trades forthis account as they are added to the Stellar ledger. If called instreaming mode, Horizon will start at the earliest known trade unless acursor is set, in which case it will start from that cursor. By settingthe cursor value to now, you can stream trades created since yourrequest time.
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
curl --location --request GET 'https://xlm.getblock.io/mainnet/accounts/GCIKZGQUUGAYKW5VR234FHNLRNGQIDDNCNPYTIUT7EGWKYKDAA6GKHCZ/trades' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_links": {
        "self": {
            "href": "https://horizon.stellar.org/accounts/GD3CJYUTZAY6JQF4CEI6Z7VW5O6VNGKZTBYUECTOJPEDTB7I2HZSPI2K/trades?cursor=&limit=3&order=asc"
        },
        "next": {
            "href": "https://horizon.stellar.org/accounts/GD3CJYUTZAY6JQF4CEI6Z7VW5O6VNGKZTBYUECTOJPEDTB7I2HZSPI2K/trades?cursor=107449584845914113-0&limit=3&order=asc"
        },
        "prev": {
            "href": "https://horizon.stellar.org/accounts/GD3CJYUTZAY6JQF4CEI6Z7VW5O6VNGKZTBYUECTOJPEDTB7I2HZSPI2K/trades?cursor=107449468881756161-0&limit=3&order=desc"
        }
    },
    "_embedded": {
        "records": [
            {
                "_links": {
                    "self": {
                        "href": ""
                    },
                    "base": {
                        "href": "https://horizon.stellar.org/accounts/GAMU5TQFUMDGVKYQPPDCD2MKKUUWELSQAEKNNU4RFQCWFSRBPJA2MAGQ"
                    },
                    "counter": {
                        "href": "https://horizon.stellar.org/accounts/GD3CJYUTZAY6JQF4CEI6Z7VW5O6VNGKZTBYUECTOJPEDTB7I2HZSPI2K"
                    },
                    "operation": {
                        "href": "https://horizon.stellar.org/operations/107449584845914113"
                    }
                },
                "id": "107449584845914113-0",
                "paging_token": "107449584845914113-0",
                "ledger_close_time": "2019-07-26T09:19:30Z",
                "trade_type": "orderbook",
                "base_offer_id": "104299223",
                "base_account": "GAMU5TQFUMDGVKYQPPDCD2MKKUUWELSQAEKNNU4RFQCWFSRBPJA2MAGQ",
                "base_amount": "748.5338945",
                "base_asset_type": "native",
                "counter_offer_id": "104299548",
                "counter_account": "GD3CJYUTZAY6JQF4CEI6Z7VW5O6VNGKZTBYUECTOJPEDTB7I2HZSPI2K",
                "counter_amount": "74.8533887",
                "counter_asset_type": "credit_alphanum4",
                "counter_asset_code": "BB1",
                "counter_asset_issuer": "GD5J6HLF5666X4AZLTFTXLY46J5SW7EXRKBLEYPJP33S33MXZGV6CWFN",
                "base_is_seller": true,
                "price": {
                    "n": "10000000",
                    "d": "100000001"
                }
            }
        ]
    }
}
```

