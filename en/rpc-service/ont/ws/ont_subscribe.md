---
title: subscribe - Ontology
description: Example code for the subscribe ws method. Сomplete guide on how to use subscribe ws in GetBlock.io Web3 documentation.
---

### Parameters


`ConstractsFilter` - array of string

optional

array of contract addresses

`SubscribeEvent` - boolean

optional

subscribe to events if true

`SubscribeJsonBlock` - boolean

optional

subscribe to json blocks if true

`SubscribeRawBlock` - boolean

optional

subscribe to raw blocksif true

`SubscribeBlockTxHashs` - boolean

optional

subscribe to transaction hashes if true

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'subscribe', 'Version': '1.0.0', 'Id': 1, 'SubscribeJsonBlock': True, 'SubscribeRawBlock': True}
```

###  Response

``` java
{
    "Action": "subscribe",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": {
        "ContractsFilter": null,
        "SubscribeBlockTxHashs": false,
        "SubscribeEvent": false,
        "SubscribeJsonBlock": true,
        "SubscribeRawBlock": true
    },
    "Version": "1.0.0"
}
```

