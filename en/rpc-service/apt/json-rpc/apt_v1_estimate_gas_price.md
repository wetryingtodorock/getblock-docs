---
title: apt:/v1/estimate_gas_price - Aptos
description: Example code for the apt:/v1/estimate_gas_price json-rpc method. Сomplete guide on how to use apt:/v1/estimate_gas_price json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


\-

### Request

``` java
curl --location --request GET 'https://apt.getblock.io/v1/estimate_gas_price?' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
```

###  Response

``` java
{
    "deprioritized_gas_estimate": 100,
    "gas_estimate": 100,
    "prioritized_gas_estimate": 150
}
```

