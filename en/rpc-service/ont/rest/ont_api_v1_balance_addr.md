---
title: ont:/api/v1/balance/{addr} \[GET\]
description: Fetches balance of a Base58 address
---

### Parameters


`addr` - path

string

Base58 encoded account address

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/balance/AQwyT6CWUNn8yKVdXpvi7wwWtEJnqri7vW' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getbalance",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": {
        "height": "16248538",
        "ong": "711911840000",
        "ont": "0"
    },
    "Version": "1.0.0"
}
```

