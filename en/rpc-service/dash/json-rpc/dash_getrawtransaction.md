---
title: dash:getrawtransaction \[POST\]
description: gets a hex-encoded serialized transaction or a JSON object describingthe transaction. By default, Dash Core only stores complete transactiondata for UTXOs and your own transactions, so the RPC may fail onhistoric transactions unless you use the non-default txindex=1 in yourDash Core startup settings.Note By default this function only works for mempool transactions. Whencalled with a blockhash argument, getrawtransaction will return thetransaction if the specified block is available and the transaction isfound in that block. When called without a blockhash argument,getrawtransaction will return the transaction if it is in the mempool,or if -txindex is enabled and the transaction is in a block in theblockchain.If you begin using txindex=1 after downloading the block chain, you mustrebuild your indexes by starting Dash Core with the option -reindex.This may take several hours to complete, during which time your nodewill not process new blocks or transactions. This reindex only needs tobe done once.
---

### Parameters


`TXID` - string (hex)

The TXID of the transaction to get, encoded as hex in RPC byte order.

`verbose` - bool

Optional.

Updated in Dash Core 0.12.3 / Bitcoin Core 0.14.0

Set to false (the default) to return the serialized transaction as hex.
Set to true to return a decoded transaction in JSON. Before 0.12.3, use
0 and 1, respectively.

`Block Hash` - bool

Optional.

Added in Dash Core 0.16.0

The hash of the block in which to look for the transaction.

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "getrawtransaction",
"params": ["83dc6c8e03026c0317885f62a7072dfde10014967f59477a0f7b5fc52f44a784", false, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "error": null,
    "id": "getblock.io",
    "result": "03000500010000000000000000000000000000000000000000000000000000000000000000ffffffff2703716d170423ce39610800004440830900000fe4b883e5bda9e7a59ee4bb99e9b1bc04f09f909f40440fa802203d5807000000001976a9147c086eada12bdb10a265c16c08a7ae87366bd48188aca03c9f08000000001976a91406c7111117f7b797528485b64772d3ffcff919ec88ac209af41f460200716d1700efc371b5251f5bae393e5962fe092f8b2003732a56eda3e1a2babe8413d17ce7ce2396a41c1f833c0cd00a0d8e900dfc4962805706e70a35074dcd30fafbd4c6"
}
```

