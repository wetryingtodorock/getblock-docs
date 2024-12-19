---
title: thetacli.NewKey  {disallowed} - Theta Network
description: Example code for the thetacli.NewKey  {disallowed} json-rpc method. Сomplete guide on how to use thetacli.NewKey  {disallowed} json-rpc in GetBlock.io Web3 documentation.
---

### Parameters


`password` - string

\-

T

h

e

p

a

s

s

w

o

r

d

f

o

r

t

h

e

n

e

w

a

c

c

o

u

n

t

.

### Request

``` java
curl --location --request POST 'https://theta.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "thetacli.NewKey",
"params": {},
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

