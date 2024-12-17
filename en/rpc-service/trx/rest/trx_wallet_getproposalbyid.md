---
title: trx:/wallet/getproposalbyid \[POST\]
description: Queries proposal based on ID and returns proposal details.
---

### Parameters


`id` - int32

`visible` - boolean

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/getproposalbyid' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"id": 80, "visible": true}'
```

###  Response

``` java
{
    "approvals": [
        "TN2W4cc7a4dsYyTLiLMWa9m7jVpdLjGvYs",
        "TGJBjL8wmRVyRStkghnhcVNYYgn6Yjno6X",
        "TDpt9adA6QidL1B1sy3D8NC717C6L5JxFo",
        "TKSXDA8HfE9E1y39RczVQ1ZascUEtaSToF",
        "TGyrSc9ZmTdbYziuk1SKEmdtCdETafewJ9",
        "TVFKwzE8qeETLaZEHMx2tjEsdnujAgAWaA",
        "TJvaAeFb8Lykt9RQcVyyTFN2iDvGMuyD4M",
        "TNaJADoq1u2atryP1ZzwvmEE4ZBELXfMqw",
        "TCEo1hMAdaJrQmvnGTCcGT2LqrGU4N7Jqf"
    ],
    "create_time": 1670906025000,
    "expiration_time": 1671170400000,
    "parameters": [
        {
            "key": 68,
            "value": 1000000
        }
    ],
    "proposal_id": 80,
    "proposer_address": "TGJBjL8wmRVyRStkghnhcVNYYgn6Yjno6X",
    "state": "APPROVED"
}
```

