---
title: rsk:eth_submitHashrate \[POST\] {disallowed}
description: Submits the mining hashrate.Used by mining software such as Ethminer.
---

### Parameters


`hashrate` - string

Hexadecimal string representation of the hash rate.

`id` - string

Random hexadecimal ID identifying the client.

### Request

``` java
wscat -c wss://rsk.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_submitHashrate",
"params": ["0x0000000000000000000000000000000000000000000000000000000000500000", "0x59daa26581d0acd1fce254fb7e85952f4c09d0915afd33d3886cd914bc7d283c"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

