---
title: eth_getUncleByBlockHashAndIndex - Ethereum
description: Example code for the eth_getUncleByBlockHashAndIndex ws method. Сomplete guide on how to use eth_getUncleByBlockHashAndIndex ws in GetBlock.io Web3 documentation.
---

### Parameters


`data` - None

32-byte block hash.

`quantity` - None

Index of the uncle.

### Request

``` java
wscat -c wss://eth.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getUncleByBlockHashAndIndex",
"params": ["0xc48fb64230a82f65a08e7280bd8745e7fea87bc7c206309dee32209fe9a985f7", "0x0"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "difficulty": "0x76b123df93230",
        "extraData": "0x50505945206e616e6f706f6f6c2e6f7267",
        "gasLimit": "0x7a121d",
        "gasUsed": "0x7a0175",
        "hash": "0xc20189c0b1a4a23116ab3b177e929137f6e826f17fc4c2e880e7258c620e9817",
        "logsBloom": "0x890086c024487ca422be846a201a10e41bc2882902312116c1119609482031e9c000e2a708004a10281024028020c505727a12570c4810121c59024490b040894406a1c23c37a0094810921da3923600c71c03044b40924280038d07ab91964a008084264a01641380798840805a284cce201a8026045451002500113a00de441001320805ca2840037000111640d090442c11116d2112948084240242340400236ce81502063401dcc214b9105194d050884721c1208800b20501a4201400276004142f118e60808284506979a86e050820101c170c185e2310005205a82a2100382422104182090184800c02489e033440218142140045801c024cc1818485",
        "miner": "0x52bc44d5378309ee2abf1539bf71de1b7d7be3b5",
        "mixHash": "0xf557cc827e058862aa3ea1bd6088fb8766f70c0eac4117c56cf85b7911f82a14",
        "nonce": "0xd320b48904347cdd",
        "number": "0x768964",
        "parentHash": "0x98d752708b3677df8f439c4529f999b94663d5494dbfc08909656db3c90f6255",
        "receiptsRoot": "0x0f838f0ceb73368e7fc8d713a7761e5be31e3b4beafe1a6875a7f275f82da45b",
        "sha3Uncles": "0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347",
        "size": "0x21a",
        "stateRoot": "0xa0c7d4fca79810c89c517eff8dadb9c6d6f4bcc27c2edfb301301e1cf7dec642",
        "timestamp": "0x5cdcbba6",
        "transactionsRoot": "0x866e38e91d01ef0387b8e07ccf35cd910224271ccf2b7477b8c8439e8b70f365",
        "uncles": []
    }
}
```

