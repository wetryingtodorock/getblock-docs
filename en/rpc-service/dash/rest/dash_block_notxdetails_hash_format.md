---
title: dash:/block/notxdetails/{hash}{format} \[GET\]
description: The block/notxdetails operation gets a block with a particular headerhash from the local block database either as a JSON object or as aserialized block. The JSON object includes TXIDs for transactions withinthe block rather than the complete transactions GET block returns.
---

### Parameters


`hash` - path

required, exactly 1

The hash of the header of the block to get, encoded as hex in RPC byte
order

`format` - path

required, exactly 1

Set to .json for decoded block contents in JSON, or .bin or hex for a
serialized block in binary or hex

### Request

``` java
curl --location --request GET 'https://dash.getblock.io/mainnet/block/notxdetails/000000000000000f190a64a90e753e02aed731731c863c47b5a1e3e3a3baf44c.json' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json'
```

###  Response

``` java
{
    "bits": "19248140",
    "cbTx": {
        "height": 1890110,
        "merkleRootMNList": "87c4a30954e2525568ae7803557d4d2aba1dbeb35936856efb2799866c4ac1f1",
        "merkleRootQuorums": "5123fc79342385bcf8615478ccb269820c5348736d27b5173f13b9d4eb7ce478",
        "version": 2
    },
    "chainlock": true,
    "chainwork": "00000000000000000000000000000000000000000000869540999ee77bd541ee",
    "confirmations": 992,
    "difficulty": 117652802.2856531,
    "hash": "000000000000000f190a64a90e753e02aed731731c863c47b5a1e3e3a3baf44c",
    "height": 1890110,
    "mediantime": 1687182569,
    "merkleroot": "c480d267bfdead2dbdd59f0b5fc82356c2f1ab7a10057c3d41120b0a03161d9b",
    "nTx": 18,
    "nextblockhash": "000000000000000f33ead801755e0b1a579da0d654de641754fc46b880018a0e",
    "nonce": 1995673787,
    "previousblockhash": "000000000000001e964b0851a48447f12a25223a636981807f1935793edb7aa7",
    "size": 19704,
    "time": 1687183171,
    "tx": [
        "964eb02db9742533bc669d0202c557337bc194786f682d69ef9688f3011497e2",
        "361617570916950c7f8252d9cb410ae2b8357daa72a1b36487627e5765ebbd4f",
        "7099f1000977d17d4a419889fc46e25554116ee3e8eef0a47797810fef6f64e3"
    ],
    "version": 536870912,
    "versionHex": "20000000"
}
```

