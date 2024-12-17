---
title: ont:getconnectioncount \[WebSocket\]
description: Fetches the number of connections to the node.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getconnectioncount', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "getconnectioncount",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": 33,
    "Version": "1.0.0"
}
```

