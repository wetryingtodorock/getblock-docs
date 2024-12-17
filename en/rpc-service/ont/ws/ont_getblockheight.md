---
title: ont:getblockheight - Ontology
description: Example code for the ont:getblockheight ws method. Сomplete guide on how to use ont:getblockheight ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getblockheight', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "getblockheight",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": 16242367,
    "Version": "1.0.0"
}
```

