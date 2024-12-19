---
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# eth\_chainId - Ethereum

{% hint style="success" %}
The Ethereum eth\_chainId method is used to obtain the unique chain ID of the connected Ethereum network.
{% endhint %}

This **Chain ID** is essential for signing transactions correctly and sending them to the appropriate Ethereum network, whether it is the **Mainnet** or test networks like **Sepolia** or **Holesky**. The **Web3 `eth_chainId`** method is a crucial part of Ethereum-based dApps and the **Core API**, allowing developers to differentiate between various Ethereum networks during JSON RPC requests.

### Supported Networks

The **`eth_chainId` RPC Ethereum** method supports the following network types

* **Mainnet**&#x20;
* **Testnet**: Sepolia, Holesky

### Parameters

{% hint style="info" %}
This method does not accept any parameters
{% endhint %}

### Request&#x20;

#### URL

{% code fullWidth="false" %}
```json
https://go.getblock.io/<ACCESS-TOKEN>/
```
{% endcode %}

To request the chain ID using the **`eth_chainId` RPC Ethereum** method via JSON-RPC, use the following **curl** command:

{% tabs %}
{% tab title="curl " %}
```json
curl --location --request POST 'https://go.getblock.io/<ACCESS-TOKEN>/' \
--header 'Content-Type: application/json' \
--data-raw '{
    "jsonrpc": "2.0",
    "method": "eth_chainId",
    "params": [],
    "id": "getblock.io"
}'
```
{% endtab %}

{% tab title="wss" %}
```powershell
wscat -c wss://eth.getblock.io/YOUR-API-KEY/ 
# wait for connection and send the request body 
{"jsonrpc": "2.0",
"method": "eth_chainId",
"params": [],
"id": "getblock.io"}
```
{% endtab %}
{% endtabs %}

### Response

A successful **`eth_chainId`** call will return the chain ID in hexadecimal format.This value can be used to verify the network:

```json
{
    "id": "getblock.io",
    "jsonrpc": "2.0",
    "result": "0x1"
}

```

### Body Params

* result: Hexadecimal representation of the Chain ID:
  * 0x1: Ethereum Mainnet
  * 0xaa36a7: Sepolia test network
  * 0x170a: Holesky test network

### Use Case

The Web3 eth\_chainId method is commonly used in Ethereum applications to verify the network ID before executing transactions. For example, when a Web3 wallet like MetaMask connects to a dApp, it uses the eth\_chainId method to confirm that the user is on the correct network (e.g., Mainnet, Sepolia, or Holesky). This helps prevent errors and ensures transactions are sent to the right block within the correct network.

**Example Scenario:**&#x49;f a user connects to a dApp using MetaMask while on an unsupported network, the dApp can use eth\_chainId to display a warning message, prompting the user to switch to the correct network, thus enhancing security and user experience.

### Code Example

Below is a Python eth\_chainId example using the requests library to send a JSON-RPC request for the eth\_chainId method

{% tabs %}
{% tab title="JavaScript" %}
```javascript
const axios = require('axios');

// Replace <ACCESS-TOKEN> with your actual API key
const url = 'https://go.getblock.io/<ACCESS-TOKEN>/';

const options = {
  method: 'POST',
  headers: {
    accept: 'application/json',
    'Content-Type': 'application/json',
  },
  data: JSON.stringify({
    id: 1,
    jsonrpc: '2.0',
    method: 'eth_chainId',
    params: [],
  }),
};

axios(url, options)
  .then((response) => {
    const chainIdHex = response.data.result; // Chain ID in Hex format
    const chainIdDec = parseInt(chainIdHex, 16); // Convert Hex to Decimal
    console.log(`Chain ID (Hex): ${chainIdHex}`);
    console.log(`Chain ID (Decimal): ${chainIdDec}`);
  })
  .catch((error) => {
    console.error('eth_chainId error:', error.message);
  });

```
{% endtab %}

{% tab title="Python" %}
```python
import requests
import json

# Define the API endpoint URL and headers
url = "https://go.getblock.io/<ACCESS-TOKEN>/"  # Replace <ACCESS-TOKEN> with your actual API token
headers = {
    "Content-Type": "application/json"
}

# Create the payload for the eth_chainId method request
payload = {
    "jsonrpc": "2.0",
    "method": "eth_chainId",
    "params": [],
    "id": "getblock.io"
}

# Send the POST request to the Ethereum node
response = requests.post(url, headers=headers, data=json.dumps(payload))

# Check if the response status code is 200 (OK)
if response.status_code == 200:
    result = response.json().get("result")
    chain_id = int(result, 16)
    print(f"Chain ID (Hex): {result}")
    print(f"Chain ID (Decimal): {chain_id}")
else:
    print("eth_chainId error:", response.status_code, response.text)

```
{% endtab %}
{% endtabs %}

The code checks for a successful HTTP response (status code 200), parses the **JSON response**, and converts the **Chain ID** from hexadecimal to decimal format. It is a core part of the **Core API** request handling for Ethereum **Endpoints**.
