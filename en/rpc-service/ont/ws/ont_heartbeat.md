---
title: heartbeat - Ontology
description: Example code for the heartbeat ws method. Сomplete guide on how to use heartbeat ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'heartbeat', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "heartbeat",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": {
        "ContractsFilter": null,
        "SubscribeBlockTxHashs": false,
        "SubscribeEvent": false,
        "SubscribeJsonBlock": false,
        "SubscribeRawBlock": false
    },
    "Version": "1.0.0"
}
```

