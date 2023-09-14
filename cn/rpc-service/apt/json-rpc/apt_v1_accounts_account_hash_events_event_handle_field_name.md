---
title: apt:/v1/accounts/{account_hash}/events/{event_handle}/{field_name} \[GET\]
description: Gets all events for a specified account, event_handle and field_name.
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
curl --location --request GET 'https://apt.getblock.io/v1/accounts/0xc20ea5a196c81d8d7aff814aa37f8a5823acffbc4193efd3b2aafc9ef2803255/events/0x1::coin::CoinStore<0x1::aptos_coin::AptosCoin>/withdraw_events?limit=10' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
[
    {
        "data": {
            "amount": "0"
        },
        "guid": {
            "account_address": "0xc20ea5a196c81d8d7aff814aa37f8a5823acffbc4193efd3b2aafc9ef2803255",
            "creation_number": "3"
        },
        "sequence_number": "0",
        "type": "0x1::coin::WithdrawEvent",
        "version": "129525896"
    }
]
```

