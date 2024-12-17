---
title: eth_getLogs - Optimism
description: Example code for the eth_getLogs ws method. Сomplete guide on how to use eth_getLogs ws in GetBlock.io Web3 documentation.
---

### Parameters


`Object` - object

The filter options

### Request

``` java
wscat -c wss://optimism.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_getLogs",
"params": [{"topics": []}],
"id": "getblock.io"}
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": [
        {
            "address": "0x94b008aa00579c1307b0ef2c499ad98a8ce58e58",
            "blockHash": "0xa5554b9292a2192c2569f7df41077fc003563133e1e5c7c73ed2050594299464",
            "blockNumber": "0x6255821",
            "data": "0x000000000000000000000000000000000000000000000000000000001eb3f4fc",
            "logIndex": "0x0",
            "removed": false,
            "topics": [
                "0xddf252ad1be2c89b69c2b068fc378daa952ba7f163c4a11628f55a4df523b3ef",
                "0x0000000000000000000000009d39fc627a6d9d9f8c831c16995b209548cc3401",
                "0x00000000000000000000000055d3cdb823ded8b5ed482a2bb1658e341731b07d"
            ],
            "transactionHash": "0xe3e14d9eaa07b65eb565d654deca82e6011b834e736e60324f14edfd5ef7b27e",
            "transactionIndex": "0x0"
        },
        {
            "address": "0x9d39fc627a6d9d9f8c831c16995b209548cc3401",
            "blockHash": "0xa5554b9292a2192c2569f7df41077fc003563133e1e5c7c73ed2050594299464",
            "blockNumber": "0x6255821",
            "data": "0x6db58959c5e606733c52d01b4aa830d61b7a02b070c64e5ef8bbaa1fdbc7960f000000000000000000000000031c67ee65e508e96c184fc8d8559b50cedebaa900000000000000000000000055d3cdb823ded8b5ed482a2bb1658e341731b07d00000000000000000000000094b008aa00579c1307b0ef2c499ad98a8ce58e58000000000000000000000000000000000000000000000000000000001eb3f4fc000000000000000000000000000000000000000000000000000000000000003827600ed272bdfbfebd8d5b4105f4dfcf8ac5e3bbdd534b8875c561ef8398d97e",
            "logIndex": "0x1",
            "removed": false,
            "topics": [
                "0x79fa08de5149d912dce8e5e8da7a7c17ccdf23dd5d3bfe196802e6eb86347c7c"
            ],
            "transactionHash": "0xe3e14d9eaa07b65eb565d654deca82e6011b834e736e60324f14edfd5ef7b27e",
            "transactionIndex": "0x0"
        }
    ]
}
```

