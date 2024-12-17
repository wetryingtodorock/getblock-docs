---
title: getsyncstatus - Ontology
description: Example code for the getsyncstatus ws method. Сomplete guide on how to use getsyncstatus ws in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0", "method": "getsyncstatus", "params": [], "id": 0}
```

###  Response

``` java
{
    "desc": "SUCCESS",
    "error": 0,
    "id": 0,
    "jsonrpc": "2.0",
    "result": {
        "CurrentBlockHeight": 16224663,
        "ConnectCount": 20,
        "MaxPeerBlockHeight": 16224663
    }
}
```

