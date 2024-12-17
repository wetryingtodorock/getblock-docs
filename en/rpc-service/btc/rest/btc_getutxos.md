---
title: btc:getutxos \[GET\]
description: The getutxo command allows querying of the UTXO set given a set of outpoints.
---

### Example

`GET /rest/getutxos/<checkmempool>/<txid>-<n>/<txid>-<n>/.../<txid>-<n>.<bin|hex|json>`

### Request

``` java
curl --location --request GET 'https://btc.getblock.io/rest/getutxos/checkmempool/b2cdfd7b89def827ff8af7cd9bff7627ff72e5e8b0f71210f92ea7a4000c5d75-0.json' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json'
```

### Response

``` java
{
   "chainHeight" : 325347,
   "chaintipHash" : "00000000fb01a7f3745a717f8caebee056c484e6e0bfe4a9591c235bb70506fb",
   "bitmap": "1",
   "utxos" : [
      {
         "height" : 2147483647,
         "value" : 8.8687,
         "scriptPubKey" : {
            "asm" : "OP_DUP OP_HASH160 1c7cebb529b86a04c683dfa87be49de35bcf589e OP_EQUALVERIFY OP_CHECKSIG",
            "hex" : "76a9141c7cebb529b86a04c683dfa87be49de35bcf589e88ac",
            "type" : "pubkeyhash",
            "address" : "mi7as51dvLJsizWnTMurtRmrP8hG2m1XvD"
         }
      }
   ]
}
```
