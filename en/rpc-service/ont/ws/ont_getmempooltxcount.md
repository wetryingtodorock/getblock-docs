---
title: getmempooltxcount - Ontology
description: Example code for the getmempooltxcount ws method. Сomplete guide on how to use getmempooltxcount ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getmempooltxcount', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "getmempooltxcount",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": [
        0,
        0
    ],
    "Version": "1.0.0"
}
```

