---
title: eth_getBlockByNumber - Huobi ECO Chain
description: Example code for the eth_getBlockByNumber ws method. Сomplete guide on how to use eth_getBlockByNumber ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - integer or string

block number or "latest", "earliest" or "pending"

`Boolean` - Boolean

If true it returns the full transaction objects, if false only the
hashes of the transactions.

### Request

``` java
wscat -c wss://heco.getblock.io/YOUR-API-KEY/mainnet/ 
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
        "baseFeePerGas": "0x0",
        "difficulty": "0x2",
        "extraData": "0xd883010202846765746888676f312e31392e35856c696e75780000000000000028e6fa02374b385cca4bbb2b0ca72236ff62c8b18256edff41dcddbe4e8b1e6123b873129a4a2d175a613c70d91c87419688bc1c41964a2d89909b57dafda48900",
        "gasLimit": "0x2625a00",
        "gasUsed": "0x19265",
        "hash": "0x48f9643e54f630e754c325b303a1b5f460cf637c4d268a31a3394bcd3db86085",
        "logsBloom": "0x00000000000000000000000000000000000000000080000000000000000000000800000000000000000000000000000000000000040000800000200000200400000000000000000000000009000000080000000000010000000000000000000008008000000000000000000000000000000000000000000000000010180000000000000000000000000000000800000000000000000200000000000000001000020000000000000000000000040004000000100004000000000000000100000000000002000000000000000000000040000000000000000008000200008000000010000001000000000000000000000000002000000000000000000000000000",
        "miner": "0x7d008abe2613ef08d3d63900973d77daa1101b3f",
        "mixHash": "0x0000000000000000000000000000000000000000000000000000000000000000",
        "nonce": "0x0000000000000000",
        "number": "0x18fd7b5",
        "parentHash": "0x23317625c18e9d6955ba20288c0dad278ad68a94e184d7cc32de397a451554e9",
        "receiptsRoot": "0x2e75cc14043027bb6727a50e1fa8319cb71c30e2aabdb9500c54bfe95e004d93",
        "sha3Uncles": "0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347",
        "size": "0x3c4",
        "stateRoot": "0x7cac5b8cabcc149a30aafdbcf38d44e5f748c037f69e00f06637fec2a22046df",
        "timestamp": "0x6476ccbf",
        "totalDifficulty": "0x31f5a68",
        "transactions": [
            "0xd9d3069fd60424e99ba529a591c8838743ec2790910a640ec9ce0dd757548fa4",
            "0x336aec4a62782682320f4172a3d091099da524935d1f5dcab07aec3ad1c998c3"
        ],
        "transactionsRoot": "0x780faa14e31daa26ba41788120db878cba51306beea170b3a2efdd9554560d26",
        "uncles": []
    }
}
```

