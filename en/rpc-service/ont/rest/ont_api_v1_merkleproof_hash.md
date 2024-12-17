---
title: ont:/api/v1/merkleproof/{hash} \[GET\]
description: Fetch merkle proof using transaction hash
---

### Parameters


`hash` - path

Tranaction hash

### Request

``` java
curl --location --request GET 'https://ont.getblock.io/mainnet/rest/api/v1/merkleproof/db81c4e00f050c4f8e2f9c7e8201fddebd18458b3c48c73c18aa0532c7b5c43c' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "Action": "getmerkleproof",
    "Desc": "SUCCESS",
    "Error": 0,
    "Result": {
        "BlockHeight": 16224161,
        "CurBlockHeight": 16248538,
        "CurBlockRoot": "4f33b035e8487f532548ef79bea22bdc03d3fb7375b3497950353af9b01451ad",
        "TargetHashes": [
            "0000000000000000000000000000000000000000000000000000000000000000",
            "2a360d47deb993cd4816fd1421f986fe49aea917c25fc500e8a74acccb0dfc85",
            "827fe233680ead7cdbe0b7e7eff743876eecc32a5d3321a415f88d765613995b",
            "4118cedbbc8ce2ef636d1aa943228bd24596390383d8162eadcfdcf029a25eb5",
            "42b970aa34e41b8bf273bd9fcc78a9f04654dfaaca2c7b4c19f9377c13ed4e0f",
            "8fe14bca99660c21a5f29ea73090978114f3c27fdacff1a869ace26f99ef4fa2"
        ],
        "TransactionsRoot": "db81c4e00f050c4f8e2f9c7e8201fddebd18458b3c48c73c18aa0532c7b5c43c",
        "Type": "MerkleProof"
    },
    "Version": "1.0.0"
}
```

