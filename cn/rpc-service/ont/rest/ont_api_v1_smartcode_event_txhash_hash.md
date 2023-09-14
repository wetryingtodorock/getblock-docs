---
title: ont:/api/v1/smartcode/event/txhash/{hash} \[GET\]
description: Fetches contract events using transaction hash
---

### Parameters


`hash` - path

Tranaction hash

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/smartcode/event/txhash/db81c4e00f050c4f8e2f9c7e8201fddebd18458b3c48c73c18aa0532c7b5c43c' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getsmartcodeeventbyhash",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": {
        "CreatedContract": "0000000000000000000000000000000000000000",
        "GasConsumed": 50000000,
        "GasStepUsed": 20000,
        "Notify": [
            {
                "ContractAddress": "e5a49d7fd57e7178e189d3965d1ee64368a1036d",
                "IsEvm": false,
                "States": [
                    "7472616e73666572",
                    "64a222d3108f3dd8a896b7a73e71b40c1e75f113",
                    "d773cd246fd21f539530d00154ed1a8b527c9591",
                    "b804b16711"
                ]
            },
            {
                "ContractAddress": "e5a49d7fd57e7178e189d3965d1ee64368a1036d",
                "IsEvm": false,
                "States": [
                    "7472616e73666572",
                    "d773cd246fd21f539530d00154ed1a8b527c9591",
                    "1ff65884aff6058a402468972865a4be03b3202e",
                    "b804b16711"
                ]
            },
            {
                "ContractAddress": "0200000000000000000000000000000000000000",
                "IsEvm": false,
                "States": [
                    "transfer",
                    "AQwyT6CWUNn8yKVdXpvi7wwWtEJnqri7vW",
                    "AFmseVrdL9f9oyCzZefL9tG6UbviEH9ugK",
                    50000000
                ]
            }
        ],
        "State": 1,
        "TxHash": "db81c4e00f050c4f8e2f9c7e8201fddebd18458b3c48c73c18aa0532c7b5c43c",
        "TxIndex": 0
    },
    "Version": "1.0.0"
}
```

