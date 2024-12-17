---
title: ont:getsessioncount \[WebSocket\]
description: Fetch session count.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getsessioncount', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "getsessioncount",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": 2,
    "Version": "1.0.0"
}
```

