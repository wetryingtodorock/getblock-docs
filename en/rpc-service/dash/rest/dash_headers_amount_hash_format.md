---
title: dash:/headers/{amount}/{hash}{format} - Dash
description: Example code for the dash:/headers/{amount}/{hash}{format} rest method. Сomplete guide on how to use dash:/headers/{amount}/{hash}{format} rest in GetBlock.io Web3 documentation.
---

### Parameters


`amount` - path

required exactly 1

The amount of block headers in upward direction to return (including the
start header hash)

`hash` - path

required exactly 1

The hash of the header of the block to get, encoded as hex in RPC byte
order

`format` - path

required exactly 1

Set to .json for decoded block contents in JSON, or .bin or hex for a
serialized block in binary or hex

### Request

``` java
curl --location --request GET 'https://dash.getblock.io/mainnet/headers/0000000000000016ede7bf00a2b9d8f73c3d68251c47568163008d3bc44ad1a6/0000000000000016ede7bf00a2b9d8f73c3d68251c47568163008d3bc44ad1a6.json' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
[
    {
        "bits": "1942efdf",
        "chainlock": true,
        "chainwork": "000000000000000000000000000000000000000000008695091d14d6adae42c9",
        "confirmations": 1002,
        "difficulty": 64163347.43326943,
        "hash": "0000000000000016ede7bf00a2b9d8f73c3d68251c47568163008d3bc44ad1a6",
        "height": 1890100,
        "mediantime": 1687181912,
        "merkleroot": "f08083fab2d5885b4b382d24234db2bc4de1a0d407498261e9fa6b8975449d87",
        "nTx": 5,
        "nextblockhash": "0000000000000022c5ed91321a38112e0108cc15799f21476d6636e14e8d7e32",
        "nonce": 3912708023,
        "previousblockhash": "0000000000000006e263d87c3193b784a61794a63720831bdb32acdf6715133d",
        "time": 1687182371,
        "version": 536870912,
        "versionHex": "20000000"
    }
]
```

