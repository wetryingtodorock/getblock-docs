---
title: /wallet/listproposals - TRON
description: Example code for the /wallet/listproposals rest method. Сomplete guide on how to use /wallet/listproposals rest in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://trx.getblock.io/wallet/listproposals' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "proposals": [
        {
            "approvals": [
                "4167e39013be3cdd3814bed152d7439fb5b6791409",
                "41e40302d6b5e889bfbd395ed884638d7f03ee3f87",
                "41c81107148e5fa4b4a2edf3d5354db6c6be5b5549",
                "41d376d829440505ea13c9d1c455317d51b62e4ab6",
                "41c5614f3ebf88785fedf9d69bd82aac1353f8b431",
                "414ce8225c8ea6c8e1e0a483132211610c765fc6df"
            ],
            "create_time": 1673933745000,
            "expiration_time": 1674194400000,
            "parameters": [
                {
                    "key": 67,
                    "value": 1
                }
            ],
            "proposal_id": 82,
            "proposer_address": "412a4d700c196a78f8ff7f0bf17d93fe6018396d2e",
            "state": "APPROVED"
        }
    ]
}
```

