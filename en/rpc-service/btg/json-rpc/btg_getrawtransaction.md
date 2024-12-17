---
title: btg:getrawtransaction \[POST\]
description: Return the raw transaction data.By default this function only works for mempool transactions. Whencalled with a blockhash argument, getrawtransaction will return thetransaction if the specified block is available and the transaction isfound in that block. When called without a blockhash argument,getrawtransaction will return the transaction if it is in the mempool,or if -txindex is enabled and the transaction is in a block in theblockchain.
---

### Parameters


`txid` - string, required

The transaction id

`verbose` - boolean, optional, default=false

If false, return a string, otherwise return a json object

`blockhash` - string, optional

The block in which to look for the transaction

### Request

``` java
curl --location --request POST 'https://btg.getblock.io/mainnet' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getrawtransaction",
"params": ["5c970c064d317658a8777ee56f192fe17d5b3afbe242d820b205c2291210f269", null, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": "010000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff320336b80a005a2d4e4f4d50212068747470733a2f2f6769746875622e636f6d2f6a6f7368756179616275742f7a2d6e6f6d70ffffffff0240be4025000000001976a9140cb60a52559620e5de9a297612d49f55f7fd14ea88ac0000000000000000266a24aa21a9ede2f61c3f71d1defd3fa999dfa36953755c690689799962b48bebd836974e8cf90120000000000000000000000000000000000000000000000000000000000000000000000000"
}
```

