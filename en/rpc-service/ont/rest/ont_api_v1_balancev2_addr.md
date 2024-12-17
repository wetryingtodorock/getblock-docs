---
title: ont:/api/v1/balancev2/{addr} \[GET\]
description: Fetch the balance of the account using an address, with ONT decimalsbeing 9, and ONG decimals being 18
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

