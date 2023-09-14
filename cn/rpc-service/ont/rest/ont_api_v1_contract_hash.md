---
title: ont:/api/v1/contract/{hash} \[GET\]
description: Fetches contract details using contract hash
---

### Parameters


`hash` - path

Contract hash

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/contract/0144587c1094f6929ed7362d6328cffff4fb4da2' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getcontract",
    "Desc": "SUCCESS",
    "Error": 0,
    "Version": "1.0.0",
    "Result": {
        "Code": "0100000000000000000000000000000000000000",
        "NeedStorage": true,
        "Name": "ONT",
        "CodeVersion": "1.0",
        "Author": "Ontology Team",
        "Email": "contact@ont.io",
        "Description": "Ontology Network ONT Token"
    }
}
```

