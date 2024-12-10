---
title: ont:getgasprice - Ontology
description: Example code for the ont:getgasprice ws method. Сomplete guide on how to use ont:getgasprice ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getgasprice', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "getgasprice",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": {
        "gasprice": 2500,
        "height": 16242369
    },
    "Version": "1.0.0"
}
```

