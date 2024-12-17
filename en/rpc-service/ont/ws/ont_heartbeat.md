---
title: ont:heartbeat \[WebSocket\]
description: Sends heartbeat information. If heartbeat information is not received bythe client the sessin expires in 5 minutes.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'heartbeat', 'Version': '1.0.0', 'Id': 1}
```

###  Response

``` java
{
    "Action": "heartbeat",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": {
        "ContractsFilter": null,
        "SubscribeBlockTxHashs": false,
        "SubscribeEvent": false,
        "SubscribeJsonBlock": false,
        "SubscribeRawBlock": false
    },
    "Version": "1.0.0"
}
```

