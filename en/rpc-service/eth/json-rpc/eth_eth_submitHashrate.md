---
title: eth:eth_submitHashrate \[POST\]
description: Submits the mining hashrate.Used by mining software such as Ethminer.
---

### Parameters


`DATA, 32 Bytes` - None

Hexadecimal string representation of the hash rate.

`DATA, 32 Bytes` - None

Random hexadecimal ID identifying the client.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_submitHashrate",
"params": ["0x500000", "0x59daa26581d0acd1fce254fb7e85952f4c09d0915afd33d3886cd914bc7d283c"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": true
}
```

