---
title: ont:/api/v1/grantong/{addr} \[GET\]
description: Fetch amount of ONG granted to an account
---

### Parameters


`addr` - path

string

Account address

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/grantong/Adj7W5Z2hTeKH7YwJsfMzLuwiD671mvJ6X' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getgrantong",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": "0",
    "Version": "1.0.0"
}
```

