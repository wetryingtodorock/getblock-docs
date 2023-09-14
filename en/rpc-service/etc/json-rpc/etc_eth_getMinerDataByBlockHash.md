---
title: etc:eth_getMinerDataByBlockHash \[POST\]
description: Returns miner data for the specified block.
---

### Parameters


`data` - string

32 byte block hash.

### Request

``` java
curl --location --request POST 'https://etc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getMinerDataByBlockHash",
"params": ["0xbb50cb8d2d5698c1b10f1a845360ecf521ff18b08f71664a4639b6bdbb08fb38"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "coinbase": "0xb68ed353ea1421668483c46dc9b872aa09ef582a",
        "difficulty": "0x00000000000000000000000000000000000000000000000000011a85f2d724c0",
        "extraData": "0x657a696c2e6d65",
        "netBlockReward": "0x0000000000000000000000000000000000000000000000004575e8cd73bed400",
        "staticBlockReward": "0x0000000000000000000000000000000000000000000000004563918244f40000",
        "totalDifficulty": "0x00000000000000000000000000000000000000000000004ca722cd36ab8b5d6c",
        "transactionFee": "0x0000000000000000000000000000000000000000000000000012574b2ecad400",
        "uncleInclusionReward": "0x0000000000000000000000000000000000000000000000000000000000000000",
        "uncleRewards": []
    }
}
```

