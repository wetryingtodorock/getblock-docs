---
title: getblocktxsbyheight - Ontology
description: Example code for the getblocktxsbyheight ws method. Сomplete guide on how to use getblocktxsbyheight ws in GetBlock.io Web3 documentation.
---

### Parameters


`Height` - int

block height

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getblocktxsbyheight', 'Version': '1.0.0', 'Id': 1, 'Height': 16241692}
```

###  Response

``` java
{
    "Action": "getblocktxsbyheight",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": {
        "Hash": "810c6b7329e664dfdd21e4a642bec16e0c8982d0c7add37e5d16bf5527206d2a",
        "Height": 16241692,
        "Transactions": [
            "3cda442a7798762de71cdbff64d6e7b8728aa5dbfa74670e1bb6ee2f0d89fdb9"
        ]
    },
    "Version": "1.0.0"
}
```

