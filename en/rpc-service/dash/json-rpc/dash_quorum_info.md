---
title: quorum_info  {disallowed} - Dash
description: Example code for the quorum_info  {disallowed} json-rpc method. Сomplete guide on how to use quorum_info  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`submethod` - string

None

`llmqType` - number

Type of quorums to list:

\- 1 - LLMQ_50_60

\- 2 - LLMQ_400_60

\- 3 - LLMQ_400_85

\- 4 - LLMQ_100_67

`quorumHash` - string (hex)

The block hash of the quorum

`includeSkShare` - bool

Optional.

Include the secret key share (default: false)

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "quorum",
"params": ["info", null, null, null],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "result": "null",
    "id": "getblock.io",
    "status_code": 405,
    "message": "Method not allowed"
}
```

