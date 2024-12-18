---
title: blocks - Bitcoin
description: Example code for the blocks rest method. Сomplete guide on how to use blocks rest in GetBlock.io Web3 documentation.
---

### Example

`GET /rest/block/<BLOCK-HASH>.<bin|hex|json>`

### Request

``` java
curl --location --request GET 'https://btc.getblock.io/rest/block/00000000c937983704a73af28acdec37b049d214adbda81d7e2a3dd146f6ed09.json' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json'
```

### Response

``` java
{
    "hash": "00000000c937983704a73af28acdec37b049d214adbda81d7e2a3dd146f6ed09", 
    "confirmations": 679033,
    "strippedsize": 216, 
    "size": 216, 
    "weight": 864, 
    "height": 1000, 
    "version": 1, 
    "versionHex": "00000001",
    "merkleroot": "fe28050b93faea61fa88c4c630f0e1f0a1c24d0082dd0e10d369e13212128f33", 
    "tx": [
        {"txid": "fe28050b93faea61fa88c4c630f0e1f0a1c24d0082dd0e10d369e13212128f33",
         "hash": "fe28050b93faea61fa88c4c630f0e1f0a1c24d0082dd0e10d369e13212128f33", 
         "version": 1, 
         "size": 135,
         "vsize": 135,
         "weight": 540, 
         "locktime": 0, 
         "vin": [
             {"coinbase": "04ffff001d02fd04", 
              "sequence": 4294967295}
         ],
         "vout": [
             {
                 "value": 50.00000000,
                 "n": 0, 
                 "scriptPubKey": {
                     "asm": "04f5eeb2b10c944c6b9fbcfff94c35bdeecd93df977882babc7f3a2cf7f5c81d3b09a68db7f0e04f21de5d4230e75e6dbe7ad16eefe0d4325a62067dc6f369446a OP_CHECKSIG",
                     "hex": "4104f5eeb2b10c944c6b9fbcfff94c35bdeecd93df977882babc7f3a2cf7f5c81d3b09a68db7f0e04f21de5d4230e75e6dbe7ad16eefe0d4325a62067dc6f369446aac",
                     "type": "pubkey"
                 }
             }
         ],
         "hex": "01000000010000000000000000000000000000000000000000000000000000000000000000ffffffff0804ffff001d02fd04ffffffff0100f2052a01000000434104f5eeb2b10c944c6b9fbcfff94c35bdeecd93df977882babc7f3a2cf7f5c81d3b09a68db7f0e04f21de5d4230e75e6dbe7ad16eefe0d4325a62067dc6f369446aac00000000"
         }
    ],
    "time": 1232346882, 
    "mediantime": 1232344831, 
    "nonce": 2595206198, 
    "bits": "1d00ffff", 
    "difficulty": 1,
    "chainwork": "000000000000000000000000000000000000000000000000000003e903e903e9", 
    "nTx": 1,
    "previousblockhash": "0000000008e647742775a230787d66fdf92c46a48c896bfbc85cdc8acc67e87d",
    "nextblockhash": "00000000a2887344f8db859e372e7e4bc26b23b9de340f725afbf2edb265b4c6"
}
```
