---
title: eth_getFilterChanges - KuCoin Community Chain
description: Example code for the eth_getFilterChanges ws method. Сomplete guide on how to use eth_getFilterChanges ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY` - string

The filter id.

### Request

``` java
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getFilterChanges",
"params": ["0x16"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        "0x1ef9f410b4f31ca45f45db1cc8ea2f00782d9108d9bb322c0c756928baddce0a",
        "0x320574a2a697d7332f220a92ed88e693796af672dd363b3196eec00a5eaebfa6"
    ]
}
```

