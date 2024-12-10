---
title: ont:getbalance - Ontology
description: Example code for the ont:getbalance ws method. Сomplete guide on how to use ont:getbalance ws in GetBlock.io Web3 documentation.
---

### Parameters


`Addr` - string

Base58 address

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getbalance', 'Version': '1.0.0', 'Id': 1, 'Addr': 'AQwyT6CWUNn8yKVdXpvi7wwWtEJnqri7vW'}
```

###  Response

``` java
{
    "Action": "getbalance",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": {
        "height": "16242367",
        "ong": "784361840000",
        "ont": "0"
    },
    "Version": "1.0.0"
}
```

