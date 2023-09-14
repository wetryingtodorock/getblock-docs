---
title: ont:getgasprice \[WebSocket\]
description: Fetch gas price.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getgasprice', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "getgasprice",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": {
        "gasprice": 2500,
        "height": 16242369
    },
    "Version": "1.0.0"
}
```

