---
title: /api/v1/balancev2/{addr} - Ontology
description: Example code for the /api/v1/balancev2/{addr} rest method. Сomplete guide on how to use /api/v1/balancev2/{addr} rest in GetBlock.io Web3 documentation.
---

### Parameters


`addr` - path

string

Base58 encoded account address

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/balancev2/AQwyT6CWUNn8yKVdXpvi7wwWtEJnqri7vW' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getbalancev2",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": {
        "height": "16248538",
        "ong": "711911840000000000000",
        "ont": "0"
    },
    "Version": "1.0.0"
}
```

