---
title: dash:quorum_verify  {disallowed} - Dash
description: Example code for the dash:quorum_verify  {disallowed} json-rpc method. Сomplete guide on how to use dash:quorum_verify  {disallowed} json-rpc in GetBlock.io Web3 documentation.
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

`id` - string (hex)

Signing request ID

`msgHash` - string (hex)

Hash of the message to be signed.

`signature` - string (hex)

Quorum signature to verify.

`quorumHash` - string (hex)

Optional.

The quorum identifier. Set to "" if you want to specify signHeight
instead.

`signHeight` - number

Optional.

The height at which the message was signed. Only works when quorumHash
is "".

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "quorum",
"params": ["verify", null, null, null, null, null, null],
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

