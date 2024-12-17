---
title: kcc:eth_getBlockByNumber \[WebSocket\]
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
wscat -c wss://kcc.getblock.io/YOUR-API-KEY/mainnet/ 
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
        "extraData": "0xd983010300846765746889676f312e31382e3130856c696e757800000000000000bc2c950b4e96b030abcfa4fde8395d08f9caa5c17f48ebe49fdc5beeda99682798c0abdebecaf02db7806f4c5ab707c32c27668c114250f63ffe5ba3d50dcc01",
        "gasLimit": "0xe4e1c0",
        "gasUsed": "0x241ea",
        "hash": "0xda87e8658ea1a5c897da845ffefd542f51943c48d4298fef200764c5496101d7",
        "logsBloom": "0x00200000000000000000400080000000000000000000000000200000000000000000000008000200000000000000000000000000000000000100200000200000000000000000000000100008000000200000000000000001000000000000000000000000000000000000000001000000000000000000000000000018000000000000000000000000004000000000000000000000400000080000005000000000060000010000000000000000000040000000000000000000000200000000000000000002000000000000000000000000000000000000001000000000000000000010000000000000000000000000000000000000000000000000000000000002",
        "miner": "0xbe5f2ffcbd26fc5304721de0c7279960c453b8f0",
        "mixHash": "0x0000000000000000000000000000000000000000000000000000000000000000",
        "nonce": "0x0000000000000000",
        "number": "0x148cdba",
        "parentHash": "0x5d0ca4239e85f5f86b38c03c8b26d905712bce5940ce6e6aeeae0e1ed1887b1c",
        "receiptsRoot": "0x41619221e3de313d4935ac5e76dfd53678f9e2eae459bc548df28eb990aac00c",
        "sha3Uncles": "0x1dcc4de8dec75d7aab85b567b6ccd41ad312451b948a7413f0a142fd40d49347",
        "size": "0x448",
        "stateRoot": "0xfd9ddb990eb698abf41f86af9db3d6b8a2675a2f8bf068bfe95ee5c0c35578ae",
        "timestamp": "0x649076be",
        "totalDifficulty": "0x29148e9",
        "transactions": [
            "0xb4c0d928f984868e447a62233d23dc3e3fb208cc11fd482805a6f3e35e4ef0a6",
            "0xc28b21847fce2676c34b2bf3102149e45001a4c02f8a4744b6941167027e250f"
        ],
        "transactionsRoot": "0xa32e6ea3611da2cd5aef7c4cde3c4c4d7bf9b00a8b6a9ad44cd06d69af5e2691",
        "uncles": []
    }
}
```

