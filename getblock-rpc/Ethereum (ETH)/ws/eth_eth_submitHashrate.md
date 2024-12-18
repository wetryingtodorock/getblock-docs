---
title: eth_submitHashrate - Ethereum
description: Example code for the eth_submitHashrate ws method. Сomplete guide on how to use eth_submitHashrate ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA, 32 Bytes` - None

Hexadecimal string representation of the hash rate.

`DATA, 32 Bytes` - None

Random hexadecimal ID identifying the client.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_submitHashrate",
"params": ["0x500000", "0x59daa26581d0acd1fce254fb7e85952f4c09d0915afd33d3886cd914bc7d283c"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": true
}
```

