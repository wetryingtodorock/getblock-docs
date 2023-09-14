---
title: btc:getrawtransaction \[POST\]
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
curl --location --request POST 'https://btc.getblock.io/mainnet/' \
--header 'x-api-key: YOUR-API-KEY' \
--header 'Content-Type: application/json' \
--data-raw '{"jsonrpc": "2.0",
"method": "getrawtransaction",
"params": ["10b54fd708ab2e5703979b4ba27ca0339882abc2062e77fbe51e625203a49642", null, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": "01000000000101e17e03d21d051aa2bd9d336c3ac0693cfa92ce71592ceec521b1c48019ff77a101000000171600146d76e574b5f4825fe740ba6c41aaf1b319dfb80cffffffff02819a010000000000160014422002d927a1cae901eac668444cce8dd0ae60d529b31b0b0000000017a914f5b48d1130dc3d366d1eabf6783a552d1c8e08f4870247304402206701306a4750908fd48dead54331a3c7b4dce04ec10bfc6dd32049e2cff061a5022013c9d66827fabbeaadeb30b41c09aca2daddf4628cd00e3b993b1c86a12ff5190121034bcb9be1daf6ce1193774d15f863768b621bc95a363f1da5810129e961a2317400000000"
}
```

