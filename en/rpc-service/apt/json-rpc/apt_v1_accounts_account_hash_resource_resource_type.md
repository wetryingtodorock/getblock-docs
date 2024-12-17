---
title: apt:/v1/accounts/{account_hash}/resource/{resource_type} \[GET\]
description: Gets a single resource for a specified account and ledger version.
---

### Parameters


`resource_type` -

A type of struct to retrieve.

`ledger_version` -

Ledger version. Defaults to latest if not provided.

### Request

``` java
curl --location --request GET 'https://apt.getblock.io/v1/accounts/0xc20ea5a196c81d8d7aff814aa37f8a5823acffbc4193efd3b2aafc9ef2803255/resource/0x1::coin::CoinStore<0x1::aptos_coin::AptosCoin>?resource_type=0x1::coin::CoinStore<0x1::aptos_coin::AptosCoin>' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "data": {
        "coin": {
            "value": "42470628935"
        },
        "deposit_events": {
            "counter": "2",
            "guid": {
                "id": {
                    "addr": "0xc20ea5a196c81d8d7aff814aa37f8a5823acffbc4193efd3b2aafc9ef2803255",
                    "creation_num": "2"
                }
            }
        },
        "frozen": false,
        "withdraw_events": {
            "counter": "1",
            "guid": {
                "id": {
                    "addr": "0xc20ea5a196c81d8d7aff814aa37f8a5823acffbc4193efd3b2aafc9ef2803255",
                    "creation_num": "3"
                }
            }
        }
    },
    "type": "0x1::coin::CoinStore<0x1::aptos_coin::AptosCoin>"
}
```

