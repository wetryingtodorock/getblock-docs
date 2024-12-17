---
title: apt:/v1/accounts/{account_hash}/events/{creation_number} - Aptos
description: Example code for the apt:/v1/accounts/{account_hash}/events/{creation_number} json-rpc method. Сomplete guide on how to use apt:/v1/accounts/{account_hash}/events/{creation_number} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`limit` -

Maximum number of events to retrieve. Gets default page size if not
provided.

`start` -

Optional starting sequence number of events. Defaults to the most recent
events.

### Request

``` java
curl --location --request GET 'https://apt.getblock.io/v1/accounts/0xc20ea5a196c81d8d7aff814aa37f8a5823acffbc4193efd3b2aafc9ef2803255/events/2?limit=10' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
[
    {
        "data": {
            "amount": "100000000000"
        },
        "guid": {
            "account_address": "0xc20ea5a196c81d8d7aff814aa37f8a5823acffbc4193efd3b2aafc9ef2803255",
            "creation_number": "2"
        },
        "sequence_number": "0",
        "type": "0x1::coin::DepositEvent",
        "version": "129456718"
    },
    {
        "data": {
            "amount": "0"
        },
        "guid": {
            "account_address": "0xc20ea5a196c81d8d7aff814aa37f8a5823acffbc4193efd3b2aafc9ef2803255",
            "creation_number": "2"
        },
        "sequence_number": "1",
        "type": "0x1::coin::DepositEvent",
        "version": "129525896"
    }
]
```

