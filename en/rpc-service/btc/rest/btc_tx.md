---
title: btc:tx \[GET\]
description: Given a transaction hash returns a transaction in binary, hex-encoded binary, or JSON formats. By default, this endpoint will only search the mempool. To query for a confirmed transaction, enable the transaction index via "txindex=1" command line/configuration option.
---

### Example

`GET /rest/tx/<TX-HASH>.<bin|hex|json>`

### Request

``` java
curl --location --request GET 'https://btc.getblock.io/rest/tx/33be25aff408d7d86a2a543af4a1440a154a7243839401a3b906d61ea72fb840.json' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json'
```

### Response

``` java
{
    "txid": "33be25aff408d7d86a2a543af4a1440a154a7243839401a3b906d61ea72fb840",
    "hash": "33be25aff408d7d86a2a543af4a1440a154a7243839401a3b906d61ea72fb840",
    "version": 1,
    "size": 367,
    "vsize": 367,
    "weight": 1468,
    "locktime": 670710,
    "vin": [
        {
            "txid": "7f3615ed6c64f34cbc98153319f2390300c8b8ca0b8658118c403feb3ec3a347",
            "vout": 0,
            "scriptSig": {
                "asm": "0 30440220154e2c770826ff6735e2c1939436be8d6643f2a1aeed035e43386d8cd68b5a6002204239ac210fdb351193990b5257c6e40e5e1d753072c4955ec928786433c6a6b8[ALL] 3044022014276a17817f0b90d7c6611be60cc4b59c277ae0db0fd1e8f10522cd26ba1bb002200f971d06e4ff0b8e7af37d95a24acd56a29c614b3e31918dd533319369bf3821[ALL] 5221025cce82dd52d843f56da52467e742f266bbc411d475815e4c9caf8fe0cfc3545c210224a43897ae8b1d84f6a8af89a51ed700bcacc6f77861c8363c136a16e18470912102638d8a81d7657b0419f996cda3d5d1e20b858f5d24d58cebf66fcb10bd83dda553ae",
                "hex": "004730440220154e2c770826ff6735e2c1939436be8d6643f2a1aeed035e43386d8cd68b5a6002204239ac210fdb351193990b5257c6e40e5e1d753072c4955ec928786433c6a6b801473044022014276a17817f0b90d7c6611be60cc4b59c277ae0db0fd1e8f10522cd26ba1bb002200f971d06e4ff0b8e7af37d95a24acd56a29c614b3e31918dd533319369bf3821014c695221025cce82dd52d843f56da52467e742f266bbc411d475815e4c9caf8fe0cfc3545c210224a43897ae8b1d84f6a8af89a51ed700bcacc6f77861c8363c136a16e18470912102638d8a81d7657b0419f996cda3d5d1e20b858f5d24d58cebf66fcb10bd83dda553ae"
            },
            "sequence": 4294967295
        }
    ],
    "vout": [
        {
            "value": 15.00000000,
            "n": 0,
            "scriptPubKey": {
                "asm": "OP_HASH160 c1adad70ace13491b95af4a1b1b200c04fd47fc2 OP_EQUAL",
                "hex": "a914c1adad70ace13491b95af4a1b1b200c04fd47fc287",
                "reqSigs": 1,
                "type": "scripthash",
                "addresses": [
                    "3KM6PteeEJKkjwPi3qdi7VeQ4EnqkFEVBs"
                ]
            }
        },
        {
            "value": 19.99984465,
            "n": 1,
            "scriptPubKey": {
                "asm": "OP_HASH160 6a0c580510463837afe2cc4f105e6cf29d81b782 OP_EQUAL",
                "hex": "a9146a0c580510463837afe2cc4f105e6cf29d81b78287",
                "reqSigs": 1,
                "type": "scripthash",
                "addresses": [
                    "3BMkLYPKBYN5CGus8ZppxXdeXMs3ZQTDJh"
                ]
            }
        }
    ],
    "hex": "010000000147a3c33eeb3f408c1158860bcab8c8000339f219331598bc4cf3646ced15367f00000000fc004730440220154e2c770826ff6735e2c1939436be8d6643f2a1aeed035e43386d8cd68b5a6002204239ac210fdb351193990b5257c6e40e5e1d753072c4955ec928786433c6a6b801473044022014276a17817f0b90d7c6611be60cc4b59c277ae0db0fd1e8f10522cd26ba1bb002200f971d06e4ff0b8e7af37d95a24acd56a29c614b3e31918dd533319369bf3821014c695221025cce82dd52d843f56da52467e742f266bbc411d475815e4c9caf8fe0cfc3545c210224a43897ae8b1d84f6a8af89a51ed700bcacc6f77861c8363c136a16e18470912102638d8a81d7657b0419f996cda3d5d1e20b858f5d24d58cebf66fcb10bd83dda553aeffffffff02002f68590000000017a914c1adad70ace13491b95af4a1b1b200c04fd47fc287515735770000000017a9146a0c580510463837afe2cc4f105e6cf29d81b78287f63b0a00"
}  
```
