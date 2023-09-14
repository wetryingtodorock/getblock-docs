---
title: ont:/api/v1/version \[GET\]
description: Fetch node version information
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/version' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getversion",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": "v2.4.3-0-gf966c6d",
    "Version": "1.0.0"
}
```

