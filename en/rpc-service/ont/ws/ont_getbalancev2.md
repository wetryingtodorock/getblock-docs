---
title: ont:getbalancev2 \[WebSocket\]
description: Fetch the balance of the account using an address, with ONTs decimalsbeing 9, a ONGs decimals being 18
---

### Parameters


`Addr` - string

Base58 address

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getbalancev2', 'Version': '1.0.0', 'Id': 1, 'Addr': 'AQwyT6CWUNn8yKVdXpvi7wwWtEJnqri7vW'}
```

###  Response

``` java
{
    "Action": "getbalancev2",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": {
        "height": "16242367",
        "ong": "784361840000000000000",
        "ont": "0"
    },
    "Version": "1.0.0"
}
```

