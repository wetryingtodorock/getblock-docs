---
title: EXPERIMENTAL_changes(all_access_key_changes)  {disallowed} - NEAR Protocol
description: >-
  Example code for the EXPERIMENTAL_changes(all_access_key_changes) 
  {disallowed} json-rpc method. Сomplete guide on how to use
  EXPERIMENTAL_changes(all_access_key_changes)  {disallowed} json-rpc in Get
---

# EXPERIMENTAL\_changes(all\_access\_key\_changes)  {disallowed} - NEAR Protocol

#### Parameters

`changes_type` - string

type of change

`finality` - string

You should pick either that or block\_id.

`block_id` - int or string

You should pick either that or finality.

The block\_id param can take either the block number OR the block hash as an argument.

`keys` - array of maps

an array of maps in format: \[{account\_id, publick\_key}]

#### Request

```java
curl --location --request POST 'https://near.getblock.io/mainnet' \ 
--header 'x-api-key: YOUR-API-KEY' \ 
--header 'Content-Type: application/json' \ 
--data-raw '{"jsonrpc": "2.0",
"method": "EXPERIMENTAL_changes",
"params": ["all_access_key_changes", "final", null, null],
"id": "getblock.io"}'
```

#### Response

```java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```
