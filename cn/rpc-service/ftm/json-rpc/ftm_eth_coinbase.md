---
title: ftm:eth_coinbase \[POST\]
description: Returns the client coinbase address. The coinbase address is the accountto pay mining rewards to.To set a coinbase address, start Besu with the --miner-coinbase optionset to a valid Ethereum account address. You can get the Ethereumaccount address from a client such as MetaMask or Etherscan.
---

### Parameters


\-

### Request

``` java
curl --location --request POST 'https://ftm.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "eth_coinbase",
"params": [],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x0000000000000000000000000000000000000000"
}
```

