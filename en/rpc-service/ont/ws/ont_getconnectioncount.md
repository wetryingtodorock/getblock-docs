---
title: ont:getconnectioncount - Ontology
description: Example code for the ont:getconnectioncount ws method. Сomplete guide on how to use ont:getconnectioncount ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getconnectioncount', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "getconnectioncount",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": 33,
    "Version": "1.0.0"
}
```

