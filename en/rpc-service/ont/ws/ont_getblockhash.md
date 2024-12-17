---
title: ont:getblockhash - Ontology
description: Example code for the ont:getblockhash ws method. Сomplete guide on how to use ont:getblockhash ws in GetBlock.io Web3 documentation.
---

### Parameters


`Height` - integer

block height

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getblockhash', 'Version': '1.0.0', 'Id': 1, 'Height': 16241692}
```

###  Response

``` java
{
    "Action": "getblockhash",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": "810c6b7329e664dfdd21e4a642bec16e0c8982d0c7add37e5d16bf5527206d2a",
    "Version": "1.0.0"
}
```

