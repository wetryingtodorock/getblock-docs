---
title: ont:getmempooltxstate - Ontology
description: Example code for the ont:getmempooltxstate ws method. Сomplete guide on how to use ont:getmempooltxstate ws in GetBlock.io Web3 documentation.
---

### Parameters


`Hash` - string

block hash

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getmempooltxstate', 'Version': '1.0.0', 'Id': 1, 'Hash': '0b437771a42d18d292741c5d4f1300a135fa6e65b0594e39dc299e7f8279221a'}
```

###  Response

``` java
{
    "Action": "getmempooltxstate",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Version": "1.0.0",
    "Result": {
        "State": [
            {
                "Type": 1,
                "Height": 342,
                "ErrCode": 0
            },
            {
                "Type": 0,
                "Height": 0,
                "ErrCode": 0
            }
        ]
    }
}
```

