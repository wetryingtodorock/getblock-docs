---
title: getsmartcodeeventbyhash - Ontology
description: Example code for the getsmartcodeeventbyhash ws method. Сomplete guide on how to use getsmartcodeeventbyhash ws in GetBlock.io Web3 documentation.
---

### Parameters


`Hash` - string

transaction hash

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getsmartcodeeventbyhash', 'Version': '1.0.0', 'Id': 1, 'Hash': '3cda442a7798762de71cdbff64d6e7b8728aa5dbfa74670e1bb6ee2f0d89fdb9'}
```

###  Response

``` java
{
    "Action": "getsmartcodeeventbyhash",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
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
                    "c5f492260bbe04a7586dc4a70081a3440f0116c9",
                    "6f0c9e3b13"
                ]
            },
            {
                "ContractAddress": "e5a49d7fd57e7178e189d3965d1ee64368a1036d",
                "IsEvm": false,
                "States": [
                    "7472616e73666572",
                    "c5f492260bbe04a7586dc4a70081a3440f0116c9",
                    "4756eba570c7c9778418a0087be9c86a45487ac0",
                    "6f0c9e3b13"
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
        "TxHash": "3cda442a7798762de71cdbff64d6e7b8728aa5dbfa74670e1bb6ee2f0d89fdb9",
        "TxIndex": 0
    },
    "Version": "1.0.0"
}
```

