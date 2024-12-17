---
title: dash:coinjoin \[POST\] {disallowed}
description: controls the CoinJoin process (previously named privatesend prior toDash Core 0.17.0).
---

### Parameters


`mode` - string

\-

'

T

h

e

c

o

m

m

a

n

d

m

o

d

e

t

o

u

s

e

:

'

\-

'

s

t

a

r

t

\-

S

t

a

r

t

C

o

i

n

J

o

i

n

'

\-

'

s

t

o

p

\-

S

t

o

p

C

o

i

n

J

o

i

n

'

\-

'

r

e

s

e

t

\-

R

e

s

e

t

C

o

i

n

J

o

i

n

'

### Request

``` java
curl --location --request POST 'https://dash.getblock.io/mainnet/' 
--header 'x-api-key: YOUR-API-KEY' 
--header 'Content-Type: application/json' 
--data-raw '{"jsonrpc": "2.0",
"method": "coinjoin",
"params": ["start"],
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

