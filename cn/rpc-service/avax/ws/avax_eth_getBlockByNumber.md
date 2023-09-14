---
title: avax:eth_getBlockByNumber \[WebSocket\]
description: Returns information about a block by block number.
---

### Parameters


`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

`Boolean` - Boolean

If true it returns the full transaction objects, if false only the
hashes of the transactions.

### Request

``` java
wscat -c wss://avax.getblock.io/YOUR-API-KEY/mainnet/ 
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
        "baseFeePerGas": "0x5e0443893",
        "blockExtraData": "0x",
        "blockGasCost": "0x61a80",
        "difficulty": "0x1",
        "extDataGasUsed": "0x0",
        "extDataHash": "0x56e81f171bcc55a6ff8345e692c0f86e5b48e01b996cadc001622fb5e363b421",
        "extraData": "0x0000000000428007000000000000000000000000001dd4470000000000340e55000000000000000000000000002b55c20000000000322c67000000000000000000000000000000000000000000000000",
        "gasLimit": "0xe4e1c0",
        "gasUsed": "0x3213ee",
        "hash": "0x3fb8949661bb2f6f5eaa5b16318d3c7e7a0990f8c2382d1fe4389e0caac6519d",
        "logsBloom": "0x0020804440002009100000108211006300064004800124882a00e02a00342110100140444000002100500400001c0000010010000001010010800210283024800041d400080080a00001000c81002028088020008046800880000100480018000004008282800c0110400010000208098200020000ca46000200009002002020440200040420000000000001108000101120081028000a08000020d0000000800284c0104100c28022020004200001000020080200080000200804000201004081001602004238040001080000000800090304420400041080010022500230001054800461e08500080100000000042c12004020001040220100100008081240",
        "miner": "0x0100000000000000000000000000000000000000",
        "mixHash": "0x0000000000000000000000000000000000000000000000000000000000000000",
        "nonce": "0x0000000000000000",
        "number": "0x1d61350",
        "parentHash": "0x325c49c63b3f894c28ee1ea9513aae8e2194e8819060cd7b888971d23a114040",
        "receiptsRoot": "0xc5533e051491f1b3218e8bc51e86c58759847916ae74ee3d4aecb1d43ae9a242",
        "sha3Uncles": "0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347",
        "size": "0x2be0",
        "stateRoot": "0xdf5aaa6e78b1fa40bbf002abeeca3bbfb8fa58a50e13dafa89d37afa71c26979",
        "timestamp": "0x6479b047",
        "totalDifficulty": "0x1d61350",
        "transactions": [
            "0x027c4627cf327e492f96c02e58d913530a7fd7436945b96fbe9a2c26fdee93ac",
            "0x0401a453052a9f6e8c698139aa7b2b08cbb20add9de59e5b9a7af411be1abd97",
            "0x3ca6ec455652733237ada0149b152a4ae0c3dce34ebc1e007c978084ed65757b",
            "0x73ac22f33120ce837d942b1748956051beafff623de668f6ac7004f94653f03e",
            "0x24149ec79a11e3c6ffb9d12f65929be2285cf154d7bfbe8c80e62588feb0bc88",
            "0x3c3e17dd2b1a0e406d23fe00bfb076303f39459159d65efcaa6a6851a62ce01b",
            "0x00e9557da2566b55fcadff69fd9d0f46c0bd5f6552d426322f6337ffdaa789d7",
            "0x5e4ca11e88acdcc5b1a8f959a5edf0b463d924cfae782d1989ca72b7a509f926",
            "0xb90dfe9406b359433e1cc070b03eb29e653b2996839788e6b40c61d76ae22f74",
            "0xbfe71dbbfeb6e1c9dcddc5bc2bb087f83ba077a5599d6606c890dfdac5bbf270",
            "0x51d770b44c905877a344d8fd3e95af18d2102754d0cacc55a359723171fd7dbb",
            "0x31a78069d9eb63b11fceb79b9534b27f5d96ce183f26a3c3907a3ff0877cc2e9",
            "0x33205cca44f19f04ec2b13ce5594b48f370dbe2dd7ea30a5723292fd56d782b6",
            "0xc6bb9fe9906f52f1ecc2bd07d2792866cb4eec310a21f2a4f1dd4022ff77ccd1",
            "0x38f20833574d7268187c53e8ffa3752764bcee49600e58d1a1b1f2b8f1c975b6",
            "0xd8e5ee25ae104fa5ba6eb6756062d815581ec0f85772f30229fc1114db4feac4",
            "0xd3fd4c19f5fbec65f7e1f2a5d376f8bf39f533fd7f3ee96237112b40227ef2e4"
        ],
        "transactionsRoot": "0x2aff3102ef3cb883265e9b93421c765714f28a70106e0a5b9d3a994cc6d60b02",
        "uncles": []
    }
}
```

