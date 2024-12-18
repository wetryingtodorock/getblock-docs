---
title: getunboundong - Ontology
description: Example code for the getunboundong ws method. Сomplete guide on how to use getunboundong ws in GetBlock.io Web3 documentation.
---

### Parameters


`Addr` - string

Base58 address

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getunboundong', 'Version': '1.0.0', 'Id': 1, 'Addr': 'AQwyT6CWUNn8yKVdXpvi7wwWtEJnqri7vW'}
```

###  Response

``` java
{
    "Action": "getunboundong",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": "10",
    "Version": "1.0.0"
}
```

