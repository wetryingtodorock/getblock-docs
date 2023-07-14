---
lastUpdated: June 10, 2023
---

# Authentication

You can authenticate using an API key to authorize your connection just like with the connection to our nodes. Please, create a new API-key in the Dashboard or use your existing one. Then, please, copy and paste the API-key to Headers or Query String.

```
curl https://api.getblock.io/external/webhook/?api_key={YOUR_API_KEY}
```

or

```
curl https://api.getblock.io/external/webhook/ -H x-api-key:{YOUR_API_KEY}
```
