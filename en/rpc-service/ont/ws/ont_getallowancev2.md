---
title: ont:getallowancev2 \[WebSocket\]
description: Return the allowance from the from account to the to account, with ONTsdecimals being 9, a ONGs decimals being 18.
---

### Parameters


`Asset` - string

asset name

`From` - string

Base58 address

`To` - string

Base58 address

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getallowancev2', 'Version': '1.0.0', 'Id': 1, 'Asset': 'ont', 'From': 'A9yD14Nj9j7xAB4dbGeiX9h8unkKHxuWwb', 'To': 'AA4WVfUB1ipHL8s3PRSYgeV1HhAU3KcKTq'}
```

###  Response

``` java
{
    "Action": "getallowance",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": "10",
    "Version": "1.0.0"
}
```

