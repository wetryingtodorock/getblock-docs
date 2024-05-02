---
lastUpdated: October 23, 2023
title: How to generate accounts and send transactions
description: Learn how to generate accounts and send transactions with GetBlock. Gain insights on account creation, transaction signing, and streamline your blockchain application development.
---

# How to generate accounts and send transactions

In this guide, the GetBlock team is going to shed light on how our users are actually getting connected to blockchain nodes. Generating accounts in blockchains and sending transactions are two first operations we would like to cover.

In blockchains, ‘account’ should be referred to as a pair of private and public keys. Blockchains ‘recognize’ their users and balances by these keypairs.

Unlike login/password pairs in traditional computational solutions, in modern blockchains, every account can be restored with a private key only.

So, to broadcast transactions to a decentralized network, we need first to create (or restore) our account.

## Creating accounts

First, we need to set an API key which is attributed to every GetBlock user. The whole set of interactions is organized via Web3.js library. In the following demo, we try to create the account in the [Binance Smart Chain](https://getblock.io/nodes/bsc/), the programmable blockchain by world-leading exchange Binance:

```javascript
const Web3 = require('web3');
const apikey = process.env['apikey'];
const network = 'testnet'; // Change to mainnet for production
const chainId = 97; // 97 is BSC testnet, 95 is BSC mainnet
const node = 'https://go.getblock.io/<ACCESS-TOKEN>/';
const web3 = new Web3(node);
// Generate new address and private key
const accountTo = web3.eth.accounts.create();
console.log(accountTo);
```

That’s how we create an account in BSC testnet. We can either generate a new account with new keypair or restore one from private key only.

```javascript
// Restore account from private key
const privateKey = process.env['privateKey'];
const accountFrom = web3.eth.accounts.privateKeyToAccount(privateKey);
```

You may ask what does ‘eth’ mean when we’re interacting with Binance Smart Chain? No mistake, it reflects the fact that Binance Smart Chain is fully compatible with Ethereum Virtual Machine.

## Sending transactions

In blockchains, transactions should be signed (authorized) to be ‘included’ into blockchains (confirmed by its consensus of miners or validators).

Here’s how our transactions are created. 0.01 ETH is used for demo.

```javascript
const createSignedTx = async (rawTx) => {
rawTx.gas = await web3.eth.estimateGas(rawTx);
return await accountFrom.signTransaction(rawTx);
}

const sendSignedTx = async (signedTx) => {
// You can use signedTx.rawTransaction as params for
// calling eth_sendRawTransaction JSON-RPC method
web3.eth.sendSignedTransaction(signedTx.rawTransaction).then(
console.log
);
}

const amountTo = "0.01" // ether
```

That’s how the transaction looks before being included in the blockchain. Once it is signed, it can be sent to miners.

```javascript
const rawTx = {
to: accountTo.address,
value: web3.utils.toWei(amountTo, 'ether'),
chainId: chainId
};

createSignedTx(rawTx).then(sendSignedTx)
```

That’s it: your account is good to go as its transaction is submitted successfully!

Should you be interested in running of forking this code, please, don’t hesitate to check it out one more time: [https://replit.com/@getblock/BSCKeyGenAndSignTx](https://replit.com/@getblock/BSCKeyGenAndSignTx)
