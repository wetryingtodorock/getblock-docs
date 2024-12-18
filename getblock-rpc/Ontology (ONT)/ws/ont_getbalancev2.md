---
title: getbalancev2 - Ontology
description: Example code for the getbalancev2 ws method. Сomplete guide on how to use getbalancev2 ws in GetBlock.io Web3 documentation.
---

### Parameters


`Addr` - string

Base58 address

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getbalancev2', 'Version': '1.0.0', 'Id': 1, 'Addr': 'AQwyT6CWUNn8yKVdXpvi7wwWtEJnqri7vW'}
```

###  Response

``` java
{
    "Action": "getbalancev2",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": {
        "height": "16242367",
        "ong": "784361840000000000000",
        "ont": "0"
    },
    "Version": "1.0.0"
}
```

