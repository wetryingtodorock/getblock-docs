---
title: ont:getversion - Ontology
description: Example code for the ont:getversion ws method. Сomplete guide on how to use ont:getversion ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getversion', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "getversion",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": "v2.4.3-0-gf966c6d",
    "Version": "1.0.0"
}
```

