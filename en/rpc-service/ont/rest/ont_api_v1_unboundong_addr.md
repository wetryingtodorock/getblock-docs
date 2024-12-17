---
title: ont:/api/v1/unboundong/{addr} \[GET\]
description: Fetch unbound ONG for an account
---

### Parameters


`addr` - path

string

account address

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/unboundong/A9yD14Nj9j7xAB4dbGeiX9h8unkKHxuWwb' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getunboundong",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": "204957950400000",
    "Version": "1.0.0"
}
```

