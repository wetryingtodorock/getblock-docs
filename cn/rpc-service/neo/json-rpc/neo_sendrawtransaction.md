---
title: neo:sendrawtransaction \[POST\]
description: Broadcasts transactions over the NEO network.
---

### Parameters


`transaction` - string

A Base64-encoded string that has been serialized after the transaction
signed in the program.

### Request

``` java
curl --location --request POST 'https://neo.getblock.io' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "sendrawtransaction",
"params": ["ALmNfAb4lqIAAAAAAAZREgAAAAAA8S8AAAEKo4e1Ppa3mJpjFDGgVt0fQKBC9gEAKQwFd29ybGQRwAwDcHV0DBR9rbALvBGpMrl7cXVBdSsPOC0EmUFifVtSAUIMQACXF48H1VRmI50ievPfC042rJgj7ZQ3Y4ff27abOpeclh+6KpsL6gWfZTAUyFOwdjkA7CWLM3HsovQeDQlI0oopDCEDzqPi+B8a+TUi0p7eTySh8L7erXKTOR0ziA9Uddl4eMkLQZVEDXg="],
"id": "getblock.io"}'
```

###  Response

``` java
{
    "hash": "0x13ccdb9f7eda95a24aa5a4841b24fed957fe7f1b944996cbc2e92a4fa4f1fa73",
    "id": "getblock.io",
    "jsonrpc": "2.0"
}
```

