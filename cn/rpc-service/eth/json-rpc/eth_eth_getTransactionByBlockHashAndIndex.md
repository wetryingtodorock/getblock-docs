---
title: eth:eth_getTransactionByBlockHashAndIndex \[POST\]
description: Returns transaction information for the specified block hash andtransaction index position.
---

### Parameters


`DATA` - None

32-byte hash of a block.

`QUANTITY` - None

Integer representing the transaction index position.

### Request

``` java
curl --location --request POST 'https://eth.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getTransactionByBlockHashAndIndex",
"params": ["0xc48fb64230a82f65a08e7280bd8745e7fea87bc7c206309dee32209fe9a985f7", "0x2"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "blockHash": "0xc48fb64230a82f65a08e7280bd8745e7fea87bc7c206309dee32209fe9a985f7",
        "blockNumber": "0x768965",
        "chainId": "0x1",
        "from": "0xb38fd09d9735a0a41bd90a12e01eaf9c2962338f",
        "gas": "0x30d40",
        "gasPrice": "0xdf8475800",
        "hash": "0xd8d81b0362c607493e737667a392182f9074f60f11d2df66c0b5d3ce00e0186b",
        "input": "0x3912521500000000000000000000000085e323e41cfff4ea8b7668f8c591dcbc6d40185e000000000000000000000000000000000000000000000000a7c3416a6470dc0000000000000000000000000000000000000000000000000000000000000000c0000000000000000000000000000000000000000000000000000000005cdcbce0000000000000000000000000000000000000000000000000000000000000496800000000000000000000000000000000000000000000000000000000000000e00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000004115835c239bcae9655b584463af1ec5b4920eed04edfeedef030a9e92ef5ef8b83032f4a209c00ea627ba6e0129f158085833348cc6f4987313f8f0eea33013391b00000000000000000000000000000000000000000000000000000000000000",
        "nonce": "0x495f",
        "r": "0x69d47969d34be198f9896dc979554093833e70c9f672410a3f7297386e2d7d91",
        "s": "0x1d3e4cb5a92a1ec5694df501d6199da69e21c426e015e52a5bb848995712d58a",
        "to": "0x560e389a2b032319e742a59ae8bafa62671089fe",
        "transactionIndex": "0x2",
        "type": "0x0",
        "v": "0x25",
        "value": "0x0"
    }
}
```

