---
title: xlm:/claimable_balances/{claimable_balance_id}/operations \[GET\]
description: This endpoint represents successful operations referencing a givenclaimable balance and can be used in streaming mode. Streaming modeallows you to listen for new operations referencing this claimablebalance as they are added to the Stellar ledger. If called in streamingmode, Horizon will start at the earliest known operation unless a cursoris set, in which case it will start from that cursor. By setting thecursor value to now, you can stream operations created since yourrequest time.
---

### Parameters


`claimable_balance_id` - path

string, required

A unique identifier for this claimable balance.

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
curl --location --request GET 'https://xlm.getblock.io/mainnet//claimable_balances/00000000178826fbfe339e1f5c53417c6fedfe2c05e8bec14303143ec46b38981b09c3f9/operations?' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "_links": {
        "self": {
            "href": "https://horizon.stellar.org/claimable_balances/00000000178826fbfe339e1f5c53417c6fedfe2c05e8bec14303143ec46b38981b09c3f9/operations?cursor=&limit=3&order=asc"
        },
        "next": {
            "href": "https://horizon.stellar.org/claimable_balances/00000000178826fbfe339e1f5c53417c6fedfe2c05e8bec14303143ec46b38981b09c3f9/operations?cursor=140648659841806337&limit=3&order=asc"
        },
        "prev": {
            "href": "https://horizon.stellar.org/claimable_balances/00000000178826fbfe339e1f5c53417c6fedfe2c05e8bec14303143ec46b38981b09c3f9/operations?cursor=140648659841806337&limit=3&order=desc"
        }
    },
    "_embedded": {
        "records": [
            {
                "_links": {
                    "self": {
                        "href": "https://horizon.stellar.org/operations/140648659841806337"
                    },
                    "transaction": {
                        "href": "https://horizon.stellar.org/transactions/fc5a98fc3869df408ebd4ac1c2e3fefec8b0a858e82ff1d14e362676708b91e8"
                    },
                    "effects": {
                        "href": "https://horizon.stellar.org/operations/140648659841806337/effects"
                    },
                    "succeeds": {
                        "href": "https://horizon.stellar.org/effects?order=desc&cursor=140648659841806337"
                    },
                    "precedes": {
                        "href": "https://horizon.stellar.org/effects?order=asc&cursor=140648659841806337"
                    }
                },
                "id": "140648659841806337",
                "paging_token": "140648659841806337",
                "transaction_successful": true,
                "source_account": "GDCJIHD3623OCYNH65UUQC3NLG2D6YCNCDPZULRLCLOA76TBQRL6A3TF",
                "type": "create_claimable_balance",
                "type_i": 14,
                "created_at": "2020-11-23T16:02:38Z",
                "transaction_hash": "fc5a98fc3869df408ebd4ac1c2e3fefec8b0a858e82ff1d14e362676708b91e8",
                "sponsor": "GDCJIHD3623OCYNH65UUQC3NLG2D6YCNCDPZULRLCLOA76TBQRL6A3TF",
                "asset": "BODHI:GDCJIHD3623OCYNH65UUQC3NLG2D6YCNCDPZULRLCLOA76TBQRL6A3TF",
                "amount": "0.1000000",
                "claimants": [
                    {
                        "destination": "GBEUDKANIFPTFHPWJ5T3R6RIO36RQBFGHYPAQ6STH7KMNDHAT36LHOLD",
                        "predicate": {
                            "unconditional": true
                        }
                    }
                ]
            }
        ]
    }
}
```

