---
title: ton:/runGetMethod \[POST\]
description: Run get method on smart contract.
---

### Parameters


`address` - body

string, required

contract address

`method` - body

integer or string, required

Method name or method id

`stack` - body

required

array of elements in format '\[\["num", int\], \["cell", cell_object\],
\["slice", slice_object\]\]'

### Request

``` java
curl --location --request POST 'https://ton.getblock.io/mainnet/rest/runGetMethod?' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{}'
```

