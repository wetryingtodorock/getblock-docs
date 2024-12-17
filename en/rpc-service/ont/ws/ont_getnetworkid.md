---
title: getnetworkid - Ontology
description: Example code for the getnetworkid ws method. Сomplete guide on how to use getnetworkid ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getnetworkid', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "getnetworkid",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": 1,
    "Version": "1.0.0"
}
```

