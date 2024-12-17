---
title: getgrantong - Ontology
description: Example code for the getgrantong ws method. Сomplete guide on how to use getgrantong ws in GetBlock.io Web3 documentation.
---

### Parameters


`Addr` - string

Base58 address

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getgrantong', 'Version': '1.0.0', 'Id': 1, 'Addr': 'AQwyT6CWUNn8yKVdXpvi7wwWtEJnqri7vW'}
```

###  Response

``` java
{
    "Action": "getgrantong",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": "0",
    "Version": "1.0.0"
}
```

