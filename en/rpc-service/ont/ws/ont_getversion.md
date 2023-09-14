---
title: ont:getversion \[WebSocket\]
description: Fetch version details for a node.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getversion', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "getversion",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": "v2.4.3-0-gf966c6d",
    "Version": "1.0.0"
}
```

