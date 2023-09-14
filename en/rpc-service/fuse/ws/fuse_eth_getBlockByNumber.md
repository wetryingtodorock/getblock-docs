---
title: fuse:eth_getBlockByNumber \[WebSocket\]
description: Returns information about a block by block number.
---

### Parameters


`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

`Boolean` - Boolean

If true it returns the full transaction objects, if false only the
hashes of the transactions.

### Request

``` java
wscat -c wss://fuse.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getBlockByNumber",
"params": ["latest", false],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "author": "0xa7ca8178558945bec5c40e6666c7ac493c9e13cc",
        "difficulty": "0xfffffffffffffffffffffffffffffffe",
        "extraData": "0xdb830303058c4f70656e457468657265756d86312e35392e30826c69",
        "gasLimit": "0x1312d00",
        "gasUsed": "0x21f94",
        "hash": "0x9b44d9c23cb804b589ccdfc9a5588332834a930e3cf44b15470392a1c8035dc2",
        "logsBloom": "0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004000000010000000000000000000000004000000000000000000000040000000000000000000200000000000000000000000000000000000000000000000000000000000000000004000000000100000000000000000000000800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000008000000000000",
        "miner": "0xa7ca8178558945bec5c40e6666c7ac493c9e13cc",
        "number": "0x167ce09",
        "parentHash": "0x0ac9ce5d0a2a95ff7b598c8828c5236a4ae5f8a7f22ae8855d9b39d6bbc30dbd",
        "receiptsRoot": "0x8798c99544289304934fa1faa8d5246a8b05ba87b6994eb529d0760f22e11834",
        "sealFields": [
            "0x841417c2d6",
            "0xb841d0ea400ebee8e7257a1cf64eefc5e69eab2c21fe8590ea028e28615f88ec1cc3134095acc84f07ac9c25dd7a83d37905cec53c822ca9df9f333b64aa15861a9d00"
        ],
        "sha3Uncles": "0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347",
        "signature": "d0ea400ebee8e7257a1cf64eefc5e69eab2c21fe8590ea028e28615f88ec1cc3134095acc84f07ac9c25dd7a83d37905cec53c822ca9df9f333b64aa15861a9d00",
        "size": "0x2dc",
        "stateRoot": "0x78c96ea641e8e9a3f24918b993ab3d903bced8720d8c2e96028850a6a94d6abe",
        "step": "337101526",
        "timestamp": "0x6476ce2e",
        "totalDifficulty": "0x167ce08ffffffffffffffffffffffffea826f21",
        "transactions": [
            "0x54126e9c78ed7c4bcd61c3c606049485576edd1c8ff30dc71869e0a2323a8563"
        ],
        "transactionsRoot": "0x17c8c9304f2cc17a1ae0e9dc3b1d993bd2cd5ca65d8f2b5d86edd4bbdc45c250",
        "uncles": []
    }
}
```

