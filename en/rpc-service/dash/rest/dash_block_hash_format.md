---
title: /block/{hash}{format} - Dash
description: Example code for the /block/{hash}{format} rest method. Сomplete guide on how to use /block/{hash}{format} rest in GetBlock.io Web3 documentation.
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
curl --location --request GET 'https://dash.getblock.io/mainnet/block/000000000000000f190a64a90e753e02aed731731c863c47b5a1e3e3a3baf44c.json?' 
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
        {
            "cbTx": {
                "height": 1890110,
                "merkleRootMNList": "87c4a30954e2525568ae7803557d4d2aba1dbeb35936856efb2799866c4ac1f1",
                "merkleRootQuorums": "5123fc79342385bcf8615478ccb269820c5348736d27b5173f13b9d4eb7ce478",
                "version": 2
            },
            "extraPayload": "02003ed71c00f1c14a6c869927fb6e853659b3be1dba2a4d7d550378ae685552e25409a3c48778e47cebd4b9133f17b5276d7348530c8269b2cc785461f8bc85233479fc2351",
            "extraPayloadSize": 70
        },
        {
            "hex": "0200000001b6613baffd1b245f61b9947328a2490c9f0e4946db90817af7aa83e40046110f000000006a473044022048713f2c0043a57274c552aec78814dbe29ec655838241dbb0ececdcedb46d7002204229defa3c5b48e50bc033744d835b4d7b4dc5cfb871639c993abba06867851f01210322f20181d186795d167ce51bb6d5d85ec93b416bfd2173082813a8eb0fbb699efeffffff022f0c8d01000000001976a914e87f6471f15fbe057b084e305a91cb4da0cf7ce788ac1a3ffa05000000001976a9142b9b4ab262df7692602bee9a502eaa3a959d10c388ac3bd71c00",
            "instantlock": true,
            "instantlock_internal": false,
            "locktime": 1890107,
            "size": 225,
            "txid": "6039d8231e846f38bf260e19affb9ecf9263c7cdb54b79e39659070e327001b6",
            "type": 0,
            "version": 2,
            "vin": [
                {
                    "scriptSig": {
                        "asm": "3044022048713f2c0043a57274c552aec78814dbe29ec655838241dbb0ececdcedb46d7002204229defa3c5b48e50bc033744d835b4d7b4dc5cfb871639c993abba06867851f[ALL] 0322f20181d186795d167ce51bb6d5d85ec93b416bfd2173082813a8eb0fbb699e",
                        "hex": "473044022048713f2c0043a57274c552aec78814dbe29ec655838241dbb0ececdcedb46d7002204229defa3c5b48e50bc033744d835b4d7b4dc5cfb871639c993abba06867851f01210322f20181d186795d167ce51bb6d5d85ec93b416bfd2173082813a8eb0fbb699e"
                    },
                    "sequence": 4294967294,
                    "txid": "0f114600e483aaf77a8190db46490e9f0c49a2287394b9615f241bfdaf3b61b6",
                    "vout": 0
                }
            ],
            "vout": [
                {
                    "n": 0,
                    "scriptPubKey": {
                        "addresses": [
                            "XwtBD8mSrxQBUCLpCqTv5w1kyA3sjUtTnz"
                        ],
                        "asm": "OP_DUP OP_HASH160 e87f6471f15fbe057b084e305a91cb4da0cf7ce7 OP_EQUALVERIFY OP_CHECKSIG",
                        "hex": "76a914e87f6471f15fbe057b084e305a91cb4da0cf7ce788ac",
                        "reqSigs": 1,
                        "type": "pubkeyhash"
                    },
                    "value": 0.26020911,
                    "valueSat": 26020911
                },
                {
                    "n": 1,
                    "scriptPubKey": {
                        "addresses": [
                            "XefQvN6UNjZMPnVgh6AW77LY6jDqpf3WRN"
                        ],
                        "asm": "OP_DUP OP_HASH160 2b9b4ab262df7692602bee9a502eaa3a959d10c3 OP_EQUALVERIFY OP_CHECKSIG",
                        "hex": "76a9142b9b4ab262df7692602bee9a502eaa3a959d10c388ac",
                        "reqSigs": 1,
                        "type": "pubkeyhash"
                    },
                    "value": 1.00286234,
                    "valueSat": 100286234
                }
            ]
        }
    ],
    "version": 536870912,
    "versionHex": "20000000"
}
```

