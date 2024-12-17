---
title: dash:/tx/{txid}{format} \[GET\]
description: The GET tx operation gets a hex-encoded serialized transaction or a JSONobject describing the transaction. By default, Dash Core only storescomplete transaction data for UTXOs and your own transactions, so thismethod may fail on historic transactions unless you use the non-defaulttxindex=1 in your Dash Core startup settings.If you begin using txindex=1 after downloading the block chain, you mustrebuild your indexes by starting Dash Core with the option -reindex.This may take several hours to complete, during which time your nodewill not process new blocks or transactions. This reindex only needs tobe done once.
---

### Parameters


`txid` - path

required exactly 1

`format` - path

required exactly 1

### Request

``` java
curl --location --request GET 'https://dash.getblock.io/mainnet/tx/964eb02db9742533bc669d0202c557337bc194786f682d69ef9688f3011497e2.json' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "blockhash": "000000000000000f190a64a90e753e02aed731731c863c47b5a1e3e3a3baf44c",
    "cbTx": {
        "height": 1890110,
        "merkleRootMNList": "87c4a30954e2525568ae7803557d4d2aba1dbeb35936856efb2799866c4ac1f1",
        "merkleRootQuorums": "5123fc79342385bcf8615478ccb269820c5348736d27b5173f13b9d4eb7ce478",
        "version": 2
    },
    "extraPayload": "02003ed71c00f1c14a6c869927fb6e853659b3be1dba2a4d7d550378ae685552e25409a3c48778e47cebd4b9133f17b5276d7348530c8269b2cc785461f8bc85233479fc2351",
    "extraPayloadSize": 70,
    "hex": "03000500010000000000000000000000000000000000000000000000000000000000000000ffffffff33033ed71c1d2f5669614254432f4d696e65642062792038393833343130393430332f1083ed670096fe0bfa6a39740950090000ffffffff02d29b4506000000001976a914bc89d6071dabc5b4494d303af761a052a5c70d5788ac11288e08000000001976a914670cd3532309b3daf5df94d429f5edea0f870e1988ac000000004602003ed71c00f1c14a6c869927fb6e853659b3be1dba2a4d7d550378ae685552e25409a3c48778e47cebd4b9133f17b5276d7348530c8269b2cc785461f8bc85233479fc2351",
    "locktime": 0,
    "size": 241,
    "txid": "964eb02db9742533bc669d0202c557337bc194786f682d69ef9688f3011497e2",
    "type": 5,
    "version": 3,
    "vin": [
        {
            "coinbase": "033ed71c1d2f5669614254432f4d696e65642062792038393833343130393430332f1083ed670096fe0bfa6a39740950090000",
            "sequence": 4294967295
        }
    ],
    "vout": [
        {
            "n": 0,
            "scriptPubKey": {
                "addresses": [
                    "XssjzLKgsfATYGqTQmiJURQzeKdpL5K1k3"
                ],
                "asm": "OP_DUP OP_HASH160 bc89d6071dabc5b4494d303af761a052a5c70d57 OP_EQUALVERIFY OP_CHECKSIG",
                "hex": "76a914bc89d6071dabc5b4494d303af761a052a5c70d5788ac",
                "reqSigs": 1,
                "type": "pubkeyhash"
            },
            "value": 1.0522517,
            "valueSat": 105225170
        }
    ]
}
```

