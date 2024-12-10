---
title: ont:getsessioncount - Ontology
description: Example code for the ont:getsessioncount ws method. Сomplete guide on how to use ont:getsessioncount ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getsessioncount', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "getsessioncount",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": 2,
    "Version": "1.0.0"
}
```

