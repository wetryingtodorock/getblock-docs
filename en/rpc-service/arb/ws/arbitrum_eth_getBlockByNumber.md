---
title: arbitrum:eth_getBlockByNumber - Arbitrum
description: Example code for the arbitrum:eth_getBlockByNumber ws method. Сomplete guide on how to use arbitrum:eth_getBlockByNumber ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

`Boolean` - Boolean

If true it returns the full transaction objects, if false only the
hashes of the transactions.

### Request

``` java
wscat -c wss://arbitrum.getblock.io/YOUR-API-KEY/mainnet/ 
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
        "baseFeePerGas": "0x5f5e100",
        "difficulty": "0x1",
        "extraData": "0xd79c44e4c3397b74b78db0ea2d34c1106d8bae0752d6e352a859ae27185dec62",
        "gasLimit": "0x4000000000000",
        "gasUsed": "0xa0d72",
        "hash": "0x17eb19de07bacbcc2a3961b8281c744707d38d7f2d10afac2f36f3bd94070c22",
        "l1BlockNumber": "0x10924a9",
        "logsBloom": "0x04000000000000000000000000000000000000000400100000200000000000000000000000000000000000000000000008000000000000000000000000000008000000000000000000000008000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000010000000000000000010010000080000000000000000000000000000000000002000400000000400000000000000000100000000000000000000000000000000000000800000000002000000000000000000000000000000000000000000000000000000000000000000000000000000200000000000000000408000000000000000000000",
        "miner": "0xa4b000000000000000000073657175656e636572",
        "mixHash": "0x000000000001310800000000010924a9000000000000000a0000000000000000",
        "nonce": "0x00000000000d7b9a",
        "number": "0x5bc416c",
        "parentHash": "0x4c11af32100851b47105994d3758551f9f4251eec103b0eab62f10e5412f7a65",
        "receiptsRoot": "0x05e9dc74ff5689786374a4a32a71fb16c799f13bfc2a17658358ef1d702f5e47",
        "sendCount": "0x13108",
        "sendRoot": "0xd79c44e4c3397b74b78db0ea2d34c1106d8bae0752d6e352a859ae27185dec62",
        "sha3Uncles": "0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347",
        "size": "0x36f",
        "stateRoot": "0xb2e63e08d3af6de03e47794664f0a1fd8e1e17c32163a7a15cc146d513d7719a",
        "timestamp": "0x6476ca1e",
        "totalDifficulty": "0x4696424",
        "transactions": [
            "0xf5254836c09ee25314eff6f19b87d4de6b32adedb2196067065c4b9b12b8385a",
            "0xcb27bd4d0715eb26077c7db009f466a43ed5da1c6de6e00421135bf946842fc1"
        ],
        "transactionsRoot": "0xe7ddc381c9baa2d8eb860080831fa7546f025581ddd3f7cbaa72ab03dc13cc8e",
        "uncles": []
    }
}
```

