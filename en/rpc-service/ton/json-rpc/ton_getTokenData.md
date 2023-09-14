---
title: ton:/getTokenData \[GET\]
description: Get NFT or Jetton information.
---

### Parameters


`address` - query

required, string

Identifier of target TON account in any form.

### Request

``` java
curl --location --request GET 'https://ton.getblock.io/mainnet/getTokenData?address=EQAG2BH0JlmFkbMrLEnyn2bIITaOSssd4WdisE4BdFMkZbir' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "ok": true,
    "result": {
        "next_item_index": 10000,
        "collection_content": {
            "type": "offchain",
            "data": "https://nft.ton.diamonds/diamonds.json"
        },
        "owner_address": "EQDsP4js-X1VVS7mBZAuoeXvKcvOYlkpsdELBHwJOez07ZTW",
        "contract_type": "nft_collection"
    }
}
```

