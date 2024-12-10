---
title: ont:/api/v1/storage/{hash}/{key} - Ontology
description: Example code for the ont:/api/v1/storage/{hash}/{key} rest method. Сomplete guide on how to use ont:/api/v1/storage/{hash}/{key} rest in GetBlock.io Web3 documentation.
---

### Parameters


`hash` - path

string

contract hash

`key` - path

string

resource key

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/storage/0144587c1094f6929ed7362d6328cffff4fb4da2/4587c1094f6' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getstorage",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": "58d15e17628000",
    "Version": "1.0.0"
}
```

