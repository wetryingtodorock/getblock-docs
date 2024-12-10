---
title: bsc:eth_getTransactionByBlockNumberAndIndex - Binance Smart Chain
description: Example code for the bsc:eth_getTransactionByBlockNumberAndIndex json-rpc method. Сomplete guide on how to use bsc:eth_getTransactionByBlockNumberAndIndex json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`QUANTITY|TAG` - hex string

Integer representing a block number or one of the string tags latest,
earliest, or pending, as described in Block Parameter.

`QUANTITY` - hex string

The transaction index position.

### Request

``` java
curl --location --request POST 'https://bsc.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_getTransactionByBlockNumberAndIndex",
"params": ["0x52A96E", "0x1"],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": {
        "blockHash": "0x94c626286c237e187454ddd993adc534f0ce3468aaec134a39fbd52185cc3a5f",
        "blockNumber": "0x52a96e",
        "from": "0x1ad3b58d09e5179e11aa4b87e5554c14cd1591b9",
        "gas": "0x647ed",
        "gasPrice": "0x6fc23ac00",
        "hash": "0x4c46b9f9d827358263e8668145ee6f38dc381a348e2d7a9b881a43aeb3c9e4c7",
        "input": "0xe86ad1470000000000000000000000000000000000000000000000000000000000000080000000000000000000000000000000000000000000000000000000000000012000000000000000000000000000000000000000000000000000000000000001a000000000000000000000000000000000000000000000042b570e6f74344000000000000000000000000000000000000000000000000000000000000000000004000000000000000000000000e9e7cea3dedca5984780bafc599bd69add087d560000000000000000000000008c784c49097dcc637b93232e15810d53871992bf000000000000000000000000bb4cdb9cbd36b01bd1cbaebf2de08d9173bc095c000000000000000000000000e9e7cea3dedca5984780bafc599bd69add087d560000000000000000000000000000000000000000000000000000000000000003000000000000000000000000bcbf0c95c94798ffef0e71a087a7e98f29d5c0ee000000000000000000000000981db69f2f2f96e0f08d6519befda0b927c221900000000000000000000000001b96b92314c44b159149f7e0303511fb2fc4774f000000000000000000000000000000000000000000000000000000000000000300000000000000000000000000000000000000000000000000000000000003e600000000000000000000000000000000000000000000000000000000000003e600000000000000000000000000000000000000000000000000000000000003e6",
        "nonce": "0xea6",
        "r": "0x43e5cd7638a4595004f88fed0382c040a06d80c1d9de650553e324f8053c3e00",
        "s": "0x4986c0200f34b41775eb83cb2ecce9519dcacff9e3a4231ea7a81ffc0eabe492",
        "to": "0xc29bbe4c7a875e113f641e66823315e5cb61d0f2",
        "transactionIndex": "0x1",
        "type": "0x0",
        "v": "0x94",
        "value": "0x0"
    }
}
```

