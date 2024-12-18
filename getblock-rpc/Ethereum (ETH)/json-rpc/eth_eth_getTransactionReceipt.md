---
title: eth_getTransactionReceipt - Ethereum
description: Example code for the eth_getTransactionReceipt json-rpc method. Сomplete guide on how to use eth_getTransactionReceipt json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - None

32-byte hash of a transaction.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getTransactionReceipt",
"params": ["0xcd718a69d478340dc28fdf6bf8056374a52dc95841b44083163ced8dfe29310c"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "blockHash": "0xe6262c1924326d12b88aaa35a95a0c7cdd11f2d20ebae84618484120bd037c34",
        "blockNumber": "0x107d7b0",
        "contractAddress": null,
        "cumulativeGasUsed": "0x19aac9a",
        "effectiveGasPrice": "0xb9029a7ea",
        "from": "0x901c7c311d39e0b26257219765e71e8db3107a81",
        "gasUsed": "0x27fb4",
        "logs": [
            {
                "address": "0xdac17f958d2ee523a2206206994597c13d831ec7",
                "blockHash": "0xe6262c1924326d12b88aaa35a95a0c7cdd11f2d20ebae84618484120bd037c34",
                "blockNumber": "0x107d7b0",
                "data": "0x0000000000000000000000000000000000000000000000000000000103f1bfef",
                "logIndex": "0x24e",
                "removed": false,
                "topics": [
                    "0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef",
                    "0x000000000000000000000000a82f91562e1cef9dec93a4ad328d01ea7827910a",
                    "0x000000000000000000000000901c7c311d39e0b26257219765e71e8db3107a81"
                ],
                "transactionHash": "0xcd718a69d478340dc28fdf6bf8056374a52dc95841b44083163ced8dfe29310c",
                "transactionIndex": "0xfc"
            },
            {
                "address": "0xb7135877cd5d40aa3b086ac6f21c51bbafbbb41f",
                "blockHash": "0xe6262c1924326d12b88aaa35a95a0c7cdd11f2d20ebae84618484120bd037c34",
                "blockNumber": "0x107d7b0",
                "data": "0x00000000000000000000000000000000000000000003f6526b99745385c00000",
                "logIndex": "0x24f",
                "removed": false,
                "topics": [
                    "0x8c5be1e5ebec7d5bd14f71427d1e84f3dd0314c0f7b2291e5b200ac8c7c3b925",
                    "0x000000000000000000000000901c7c311d39e0b26257219765e71e8db3107a81",
                    "0x000000000000000000000000000000000022d473030f116ddee9f6b43ac78ba3"
                ],
                "transactionHash": "0xcd718a69d478340dc28fdf6bf8056374a52dc95841b44083163ced8dfe29310c",
                "transactionIndex": "0xfc"
            },
            {
                "address": "0xb7135877cd5d40aa3b086ac6f21c51bbafbbb41f",
                "blockHash": "0xe6262c1924326d12b88aaa35a95a0c7cdd11f2d20ebae84618484120bd037c34",
                "blockNumber": "0x107d7b0",
                "data": "0x000000000000000000000000000000000000000000000a968163f0a57b400000",
                "logIndex": "0x250",
                "removed": false,
                "topics": [
                    "0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef",
                    "0x000000000000000000000000901c7c311d39e0b26257219765e71e8db3107a81",
                    "0x000000000000000000000000a82f91562e1cef9dec93a4ad328d01ea7827910a"
                ],
                "transactionHash": "0xcd718a69d478340dc28fdf6bf8056374a52dc95841b44083163ced8dfe29310c",
                "transactionIndex": "0xfc"
            },
            {
                "address": "0xa82f91562e1cef9dec93a4ad328d01ea7827910a",
                "blockHash": "0xe6262c1924326d12b88aaa35a95a0c7cdd11f2d20ebae84618484120bd037c34",
                "blockNumber": "0x107d7b0",
                "data": "0x000000000000000000000000000000000000000000000a968163f0a57b400000fffffffffffffffffffffffffffffffffffffffffffffffffffffffefc0e40110000000000000000000000000000000000000000000004f77993b72687d0b8d40000000000000000000000000000000000000000000000002672ab0fa51842cafffffffffffffffffffffffffffffffffffffffffffffffffffffffffffb6981",
                "logIndex": "0x251",
                "removed": false,
                "topics": [
                    "0xc42079f94a6350d7e6235f29174924f928cc2ac818eb64fed8004e115fbcca67",
                    "0x000000000000000000000000ef1c6e67703c7bd7107eed8303fbe6ec2554bf6b",
                    "0x000000000000000000000000901c7c311d39e0b26257219765e71e8db3107a81"
                ],
                "transactionHash": "0xcd718a69d478340dc28fdf6bf8056374a52dc95841b44083163ced8dfe29310c",
                "transactionIndex": "0xfc"
            }
        ],
        "logsBloom": "0x00000000000000000000000000000000000000000000000000001000000000000000000000000000000000000000010000000000800020000000000000200000000040000000000800104008000000000000000000000800000000001200000000000000000000000000000000000000000000000020000000020010000800000000000000000000000000000000000000000000000000000000000000120000020800000000000000100084000000000000000000000000000000000000000000000002000000000000001000000000400000000000000000000000000000000010000000000000000000000000000000000000000000000000000090000000",
        "status": "0x1",
        "to": "0xef1c6e67703c7bd7107eed8303fbe6ec2554bf6b",
        "transactionHash": "0xcd718a69d478340dc28fdf6bf8056374a52dc95841b44083163ced8dfe29310c",
        "transactionIndex": "0xfc",
        "type": "0x2"
    }
}
```

