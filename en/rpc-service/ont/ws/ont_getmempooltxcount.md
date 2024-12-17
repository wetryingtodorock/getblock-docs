---
title: ont:getmempooltxcount \[WebSocket\]
description: Fetch the transaction count in the memory pool.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getmempooltxcount', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "getmempooltxcount",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": [
        0,
        0
    ],
    "Version": "1.0.0"
}
```

