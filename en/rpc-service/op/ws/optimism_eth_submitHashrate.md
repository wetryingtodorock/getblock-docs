---
title: eth_submitHashrate  {disallowed} - Optimism
description: Example code for the eth_submitHashrate  {disallowed} ws method. Сomplete guide on how to use eth_submitHashrate  {disallowed} ws in GetBlock.io Web3 documentation.
---

### Parameters


`hashrate` - string

Hexadecimal string representation of the hash rate.

`id` - string

Random hexadecimal ID identifying the client.

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
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

