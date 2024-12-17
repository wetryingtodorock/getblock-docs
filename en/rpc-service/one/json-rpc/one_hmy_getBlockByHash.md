---
title: one:hmy_getBlockByHash - Harmony
description: Example code for the one:hmy_getBlockByHash json-rpc method. Сomplete guide on how to use one:hmy_getBlockByHash json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`DATA` - hex string

32-byte hash of a block.

`Boolean` - boolean

If true, returns the full transaction objects; if false, returns the
transaction hashes.

### Request

``` java
curl --location --request POST 'https://one.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "hmy_getBlockByHash",
"params": ["0x910c18611575d42685a4d122a71c9d359a68c3f9786e1ca5a18c27819f8504ff", false],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "difficulty": 0,
        "epoch": "0x5ba",
        "extraData": "0x",
        "gasLimit": "0x4c4b400",
        "gasUsed": "0x38fcd",
        "hash": "0x910c18611575d42685a4d122a71c9d359a68c3f9786e1ca5a18c27819f8504ff",
        "logsBloom": "0x00200000010000000000000080020000000001000000100000000000020042000000010000000010000000000000080000020000000000000000000000000000000000000040008000000008000000200000400000000000000000000000000000000000000000001040000000000001000000000000000000900010000000100000000800000000000000000000000000000000000000080000004000000000000000000000000000000000000000000000080000004000080000000002000000000022000400008000000000000800000000000000001000000000000000000000000000000002080000000000000000082000000000000000000000000000",
        "miner": "one1gh043zc95e6mtutwy5a2zhvsxv7lnlklkj42ux",
        "mixHash": "0x0000000000000000000000000000000000000000000000000000000000000000",
        "nonce": 0,
        "number": "0x286a84d",
        "parentHash": "0x6b88f665d66fa9110d599dd00a419d1ad1920e858b21d840192634c146729476",
        "receiptsRoot": "0xd994ef6ad428d85c89637d8aecdad842cfaf1b80f555fbfe14cb34bd50fa8240",
        "size": "0x882",
        "stakingTransactions": [],
        "stateRoot": "0x5ba573396e3acc4bf108f303de8bde9f8a619f21efbdc266f984ac7b72b5237c",
        "timestamp": "0x647409e5",
        "transactions": [
            "0xef7ec4991840bd66569fa070ea9ab39b38a2233bbc5b3cfd272fa456e893b135"
        ],
        "transactionsInEthHash": [
            "0x48a4124c61f3e81f8a3fe7b885a6705e8096343ece3bac530dc88a864c9c0439"
        ],
        "transactionsRoot": "0x036f9e5dfe250b23eae028edf25d071c03a9bd09a6bb03953e916e1e662d1c63",
        "uncles": [],
        "viewID": "0x286b8ab",
        "vrf": "0xf97d3193f7aaa79d4f84c10b066c43faf2aa2f82f64581131ad03ed85c1911fc",
        "vrfProof": "0x81bcb4fcac5f878aacdb172ad31e878694edb606ba95c448319b992c860d7039f0596db45180362ece1641d9e7a2a90328e11f0579ad174f7e64b37b8ab9dfad3b934dde314bb71688c9bee68297abfa6ecc67cdffc95179b139f15b62330481"
    }
}
```

