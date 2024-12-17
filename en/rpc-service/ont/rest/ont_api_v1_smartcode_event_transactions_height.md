---
title: ont:/api/v1/smartcode/event/transactions/{height} \[GET\]
description: Fetch contract execution result using block height
---

### Parameters


`height` - path

integer

block height

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/smartcode/event/transactions/16242872' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getsmartcodeeventbyheight",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": [
        {
            "CreatedContract": "0000000000000000000000000000000000000000",
            "GasConsumed": 70000000,
            "GasStepUsed": 20000,
            "Notify": [
                {
                    "ContractAddress": "e5a49d7fd57e7178e189d3965d1ee64368a1036d",
                    "IsEvm": false,
                    "States": [
                        "7472616e73666572",
                        "64a222d3108f3dd8a896b7a73e71b40c1e75f113",
                        "4565cd4515630e0f8a3e2d8241be2ec21e8e1595",
                        "7eafe1e214"
                    ]
                },
                {
                    "ContractAddress": "e5a49d7fd57e7178e189d3965d1ee64368a1036d",
                    "IsEvm": false,
                    "States": [
                        "7472616e73666572",
                        "4565cd4515630e0f8a3e2d8241be2ec21e8e1595",
                        "e75e06f58cf3868f94a036c8622448806bd9a0da",
                        "7eafe1e214"
                    ]
                },
                {
                    "ContractAddress": "0200000000000000000000000000000000000000",
                    "IsEvm": false,
                    "States": [
                        "transfer",
                        "AQwyT6CWUNn8yKVdXpvi7wwWtEJnqri7vW",
                        "AFmseVrdL9f9oyCzZefL9tG6UbviEH9ugK",
                        70000000
                    ]
                }
            ],
            "State": 1,
            "TxHash": "fb8660eee2cd98a8683daf4e06e0180b470896d68f6b8a4e4dffb1f18f68ff49",
            "TxIndex": 0
        }
    ],
    "Version": "1.0.0"
}
```

