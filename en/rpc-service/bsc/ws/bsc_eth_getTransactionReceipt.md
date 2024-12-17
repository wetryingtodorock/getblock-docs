---
title: bsc:eth_getTransactionReceipt - Binance Smart Chain
description: Example code for the bsc:eth_getTransactionReceipt ws method. Сomplete guide on how to use bsc:eth_getTransactionReceipt ws in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - hex string

32-byte hash of a transaction.

### Request

``` java
wscat -c wss://bsc.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getTransactionReceipt",
"params": ["0xfdfe964c83a3b5b4625697522c7e8f4107bb7fbcd869022a4555ff554cc1504f"],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "blockHash": "0x6e6a058ac35224a9842a8010042ddc93dea2f073260a8d79cd3368a232c3e7ed",
        "blockNumber": "0x1afe984",
        "contractAddress": null,
        "cumulativeGasUsed": "0x89172b",
        "effectiveGasPrice": "0x0",
        "from": "0x2465176c461afb316ebc773c61faee85a6515daa",
        "gasUsed": "0x6a20",
        "logs": [
            {
                "address": "0x0000000000000000000000000000000000001000",
                "blockHash": "0x6e6a058ac35224a9842a8010042ddc93dea2f073260a8d79cd3368a232c3e7ed",
                "blockNumber": "0x1afe984",
                "data": "0x000000000000000000000000000000000000000000000000000a9c0abb423b9f",
                "logIndex": "0xc1",
                "removed": false,
                "topics": [
                    "0x627059660ea01c4733a328effb2294d2f86905bf806da763a89cee254de8bee5"
                ],
                "transactionHash": "0xfdfe964c83a3b5b4625697522c7e8f4107bb7fbcd869022a4555ff554cc1504f",
                "transactionIndex": "0x99"
            },
            {
                "address": "0x0000000000000000000000000000000000001000",
                "blockHash": "0x6e6a058ac35224a9842a8010042ddc93dea2f073260a8d79cd3368a232c3e7ed",
                "blockNumber": "0x1afe984",
                "data": "0x000000000000000000000000000000000000000000000000005f7c609554189d",
                "logIndex": "0xc2",
                "removed": false,
                "topics": [
                    "0x93a090ecc682c002995fad3c85b30c5651d7fd29b0be5da9d784a3302aedc055",
                    "0x0000000000000000000000002465176c461afb316ebc773c61faee85a6515daa"
                ],
                "transactionHash": "0xfdfe964c83a3b5b4625697522c7e8f4107bb7fbcd869022a4555ff554cc1504f",
                "transactionIndex": "0x99"
            }
        ],
        "logsBloom": "0x00000000000000000000000000000000000000000000000000000000000000000000002000000000000000000000000000000000000000000000001000000000000000000000000000000000000000002010000000000000000000000000000000000020000200000000000000000000080000000000000000000000000000000000000000000000000000000000000000000400000000000000000000000020000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000002000000000000000000000000010000000000020000000000000000000000000000000000",
        "status": "0x1",
        "to": "0x0000000000000000000000000000000000001000",
        "transactionHash": "0xfdfe964c83a3b5b4625697522c7e8f4107bb7fbcd869022a4555ff554cc1504f",
        "transactionIndex": "0x99",
        "type": "0x0"
    }
}
```

