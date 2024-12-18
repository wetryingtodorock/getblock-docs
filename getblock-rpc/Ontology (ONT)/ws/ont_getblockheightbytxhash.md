---
title: getblockheightbytxhash - Ontology
description: Example code for the getblockheightbytxhash ws method. Сomplete guide on how to use getblockheightbytxhash ws in GetBlock.io Web3 documentation.
---

### Parameters


`Hash` - string

transaction hash

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getblockheightbytxhash', 'Version': '1.0.0', 'Id': 1, 'Hash': '3cda442a7798762de71cdbff64d6e7b8728aa5dbfa74670e1bb6ee2f0d89fdb9'}
```

###  Response

``` java
{
    "Action": "getblockheightbytxhash",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": 16241692,
    "Version": "1.0.0"
}
```

