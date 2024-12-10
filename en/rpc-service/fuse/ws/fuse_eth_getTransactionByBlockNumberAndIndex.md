---
title: fuse:eth_getTransactionByBlockNumberAndIndex - Fuse Network
description: Example code for the fuse:eth_getTransactionByBlockNumberAndIndex ws method. Сomplete guide on how to use fuse:eth_getTransactionByBlockNumberAndIndex ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

`QUANTITY` - integer

Transaction index position.

### Request

``` java
wscat -c wss://fuse.getblock.io/YOUR-API-KEY/mainnet/ 
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
        "blockHash": "0xecaf26dbede6b144ccb4e7ea890e8564fba5a44e8ed7af0965ab8eb53518a558",
        "blockNumber": "0x167ce0a",
        "chainId": "0x7a",
        "condition": null,
        "creates": null,
        "from": "0x0c371f68c499e5af1e5e88521271dd8de498f7e0",
        "gas": "0x3f64b",
        "gasPrice": "0x2540be400",
        "hash": "0xabb73bf42177ff400c611b7010a2c4f54cfa656dd4c87e9b0c4dcf0d1630cb89",
        "input": "0x4e71d92d",
        "nonce": "0x157",
        "publicKey": "0xb6b78615fd4209638a3589340f6c56d88be3f720b9b91431f1460a489dfb69e9a59714747b828000643246e1cf92b2c4612f8e4987cf76aa58404869401560af",
        "r": "0x1a0391ccffe8fd3f6387a79b446cd877aab9c0425bab41920e80a8b214100bd5",
        "raw": "0xf86d8201578502540be4008303f64b94d253a5203817225e9768c05e5996d642fb96ba8680844e71d92d820118a01a0391ccffe8fd3f6387a79b446cd877aab9c0425bab41920e80a8b214100bd5a03dbdc2c69d2da89346afb981de64fc930d8cdf8e718145993a3ad0cfe6ad786a",
        "s": "0x3dbdc2c69d2da89346afb981de64fc930d8cdf8e718145993a3ad0cfe6ad786a",
        "standardV": "0x1",
        "to": "0xd253a5203817225e9768c05e5996d642fb96ba86",
        "transactionIndex": "0x0",
        "type": "0x0",
        "v": "0x118",
        "value": "0x0"
    }
}
```

