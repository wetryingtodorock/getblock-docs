---
title: /wallet/gettransactioninfobyblocknum - TRON
description: Example code for the /wallet/gettransactioninfobyblocknum rest method. Сomplete guide on how to use /wallet/gettransactioninfobyblocknum rest in GetBlock.io Web3 documentation.
---

### Parameters


`num` - int32

Block height.

### Request

``` java
curl --location --request POST 'https://trx.getblock.io/wallet/gettransactioninfobyblocknum' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"num": 30864600}'
```

###  Response

``` java
[
    {
        "blockNumber": 30864600,
        "blockTimeStamp": 1623056091000,
        "contractResult": [
            ""
        ],
        "id": "8971d5c2c3b45dee02860ce821e9c2ba601424c311a7a80545848a4c4c09b4a1",
        "receipt": {
            "net_usage": 283
        }
    },
    {
        "blockNumber": 30864600,
        "blockTimeStamp": 1623056091000,
        "contractResult": [
            "0000000000000000000000000000000000000000000000000000000000000000"
        ],
        "contract_address": "41a614f803b6fd780986a42c78ec9c7f77e6ded13c",
        "id": "0af79242191c6728b79e858a36a4b5c65e4e52b9fcee4dc5af30eac57b6d0953",
        "log": [
            {
                "address": "a614f803b6fd780986a42c78ec9c7f77e6ded13c",
                "data": "000000000000000000000000000000000000000000000000000000001fb6e57f",
                "topics": [
                    "ddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef",
                    "000000000000000000000000e4b8075df69297bc24cc4bbaf48cd17206e1f62c",
                    "0000000000000000000000000d0707963952f2fba59dd06f2b425ace40b492fe"
                ]
            }
        ],
        "receipt": {
            "energy_usage": 10727,
            "energy_usage_total": 14631,
            "net_usage": 338,
            "origin_energy_usage": 3904,
            "result": "SUCCESS"
        }
    }
]
```

