---
title: ont:/api/v1/allowance/{asset}/{from}/{to} \[GET\]
description: Fetches amount of allowance of an asset from one account to another
---

### Parameters


`asset` - path

string

Asset contract hash

`from` - path

string

Source account address

`to` - path

string

Recipient account address

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/allowance/ont/A9yD14Nj9j7xAB4dbGeiX9h8unkKHxuWwb/AA4WVfUB1ipHL8s3PRSYgeV1HhAU3KcKTq' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getallowance",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": "10",
    "Version": "1.0.0"
}
```

