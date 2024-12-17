---
title: heco:eth_getTransactionByBlockNumberAndIndex - Huobi ECO Chain
description: Example code for the heco:eth_getTransactionByBlockNumberAndIndex ws method. Сomplete guide on how to use heco:eth_getTransactionByBlockNumberAndIndex ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

`QUANTITY` - integer

Transaction index position.

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getTransactionByBlockNumberAndIndex",
"params": ["latest", "0x0"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "blockHash": "0x48f9643e54f630e754c325b303a1b5f460cf637c4d268a31a3394bcd3db86085",
        "blockNumber": "0x18fd7b5",
        "from": "0xf86e6ea39ad260fce4e82a5a575e894f53422dfe",
        "gas": "0x14332",
        "gasPrice": "0x938580c0",
        "hash": "0xd9d3069fd60424e99ba529a591c8838743ec2790910a640ec9ce0dd757548fa4",
        "input": "0xa9059cbb000000000000000000000000c05c77ae2cd43142aaf5b29b10255c336f9ca65500000000000000000000000000000000000000000000001043561a8829300000",
        "nonce": "0x7f",
        "r": "0x944ddc7d4c64af04f3e84033aae7e87678aa961f219a5592b42d8d8022f3b329",
        "s": "0x35916583b7a9041a333e8c15611f88c3ba8095c548c6679b8aa14cb9fd66cee0",
        "to": "0xa71edc38d189767582c38a3145b5873052c3e47a",
        "transactionIndex": "0x0",
        "type": "0x0",
        "v": "0x123",
        "value": "0x0"
    }
}
```

