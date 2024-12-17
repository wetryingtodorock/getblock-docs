---
title: getstorage - Ontology
description: Example code for the getstorage ws method. Сomplete guide on how to use getstorage ws in GetBlock.io Web3 documentation.
---

### Parameters


`Hash` - string

contract hash

`Key` - string

storage key

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getstorage', 'Version': '1.0.0', 'Id': 1, 'Hash': '0144587c1094f6929ed7362d6328cffff4fb4da2', 'Key': '4587c1094f6'}
```

###  Response

``` java
{
    "Action": "getstorage",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": "58d15e17628000",
    "Version": "1.0.0"
}
```

