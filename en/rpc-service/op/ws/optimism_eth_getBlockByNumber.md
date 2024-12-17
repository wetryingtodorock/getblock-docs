---
title: eth_getBlockByNumber - Optimism
description: Example code for the eth_getBlockByNumber ws method. Сomplete guide on how to use eth_getBlockByNumber ws in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - string

block number or "latest", "earliest" or "pending"

`Boolean` - Boolean

If true it returns the full transaction objects, if false only the
hashes of the transactions.

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
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
        "difficulty": "0x2",
        "extraData": "0xd98301090a846765746889676f312e31352e3133856c696e7578000000000000cf2ada30ff8b6f9aa3b4a15ac0bf7a088a493e18b4a0de1cb14a2672e0f4758d31660579eb550bacf1ed3a3f05a79911e5c900fd1331f8bb51a044eb7197921e00",
        "gasLimit": "0xe4e1c0",
        "gasUsed": "0x31735",
        "hash": "0xa5554b9292a2192c2569f7df41077fc003563133e1e5c7c73ed2050594299464",
        "logsBloom": "0x00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002000000000000000000040000004000100000001000000000000000008008000000000000000000000000000100000000000000000004000000000000000000000000002000000000000000000010000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000010000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000000000000000000000800001000000000800000800000000000000008000000000000000000",
        "miner": "0x0000000000000000000000000000000000000000",
        "mixHash": "0x0000000000000000000000000000000000000000000000000000000000000000",
        "nonce": "0x0000000000000000",
        "number": "0x6255821",
        "parentHash": "0x1b73e37d442d522ed9b8dca1b18ef45192aae1afcbd6b66518ff6f42ff0f6455",
        "receiptsRoot": "0x828681703016971aa0ca912fa402d1bccced1394d6ad4af7c65155b7d9eff466",
        "sha3Uncles": "0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347",
        "size": "0xe55",
        "stateRoot": "0x1b02a89e0a2db4d9f9aa311b5649a1c2e5941fb3a46ea20a887ac6bd27c2cad6",
        "timestamp": "0x6476c824",
        "totalDifficulty": "0xc4ab043",
        "transactions": [
            "0xe3e14d9eaa07b65eb565d654deca82e6011b834e736e60324f14edfd5ef7b27e"
        ],
        "transactionsRoot": "0xc9cdc1f518c1299f37e063a1babdc29893648d9105894bc52794783c37c1218e",
        "uncles": []
    }
}
```

