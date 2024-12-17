---
title: ont:getmerkleproof - Ontology
description: Example code for the ont:getmerkleproof ws method. Сomplete guide on how to use ont:getmerkleproof ws in GetBlock.io Web3 documentation.
---

### Parameters


`Hash` - string

block hash

### Request

``` java
wscat -c wss://ont.getblock.io/YOUR-API-KEY/mainnet/ 
# wait for connection and send the request body 
{'Action': 'getmerkleproof', 'Version': '1.0.0', 'Id': 1, 'Hash': '810c6b7329e664dfdd21e4a642bec16e0c8982d0c7add37e5d16bf5527206d2a'}
```

###  Response

``` java
{
    "Action": "getmerkleproof",
    "Desc": "SUCCESS",
    "Error": 0,
    "Id": 1,
    "Result": {
        "Type": "MerkleProof",
        "TransactionsRoot": "fe3a4ee8a44e3e588de55de1b8fe08f08b6184d9c062cf7316fb9481eb57b9e6",
        "BlockHeight": 16241692,
        "CurBlockRoot": "57476eba688531dec8555cb712835c7eda48a478431a2cfd3372aeee5298e711",
        "CurBlockHeight": 16241692,
        "TargetHashes": [
            "270cd10ea235cc18cba83a070fdf18ae576983b6b9a7bb9a3fec540b3786c85c",
            "24e4697f9dd6cb944d0736bd3e11b64f64edec94fb599e25d4e5461d54174f0e",
            "9a47ab04acf6bba7bb97b83eddeb0db20e11c0627b8079b40b60031d5bd63154",
            "d1b513810b9b983014c9f8b7084b8ea8744eca8e7c942586c2b7c63f910363ca"
        ]
    },
    "Version": "1.0.0"
}
```

