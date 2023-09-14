---
title: xlm:/claimable_balances/{claimable_balance_id} \[GET\]
description: The single claimable balance endpoint provides information on aclaimable balance.
---

### Parameters


`claimable_balance_id` - path

string, required

A unique identifier for this claimable balance.

### Request

``` java
curl --location --request GET 'https://xlm.getblock.io/mainnet/claimable_balances/00000000446bbc79c503c759275d433b088a89b122981ff104a76bc4fdb8e212a87eae35' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
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
```

