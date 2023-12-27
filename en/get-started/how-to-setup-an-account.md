---
lastUpdated: October 24, 2023
---

# How to set up an account

To start using the GetBlock node connection services for building a decentralized application (dApp), an account should be registered and customized. It only takes a few clicks!

## Step 1. Signing up to GetBlock

Please, select a preferred sign-up option:

- Connect wallet. By choosing this option, you are not required to share your email address and create a new password. If you do not currently have a wallet browser extension, you will be asked to install the extension.
- Sign in with Google. Google will share your name, email address, language preference, and profile picture with getblock.io.
- Sign up with email. You will be asked to provide your name and email address. Should you choose the first option, you’ll be asked to verify the email address you entered.

Note that to start using our service you will be asked to accept our [Terms of Service](https://getblock.io/terms-of-service/) and [Privacy Policy](https://getblock.io/privacy-policy/).

![screenshot 1](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_1.webp)

## Step 2. Check your user ID.

Find your user ID located in the ‘Account Settings’ section. Please use it when contacting GetBlock’s team so we can identify your account and help you faster.

![screenshot 2](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_2.webp)

## Step 3. Choose your way to interact with blockchain

With [shared nodes](https://getblock.io/nodes/), users can access peer-shared node infrastructure. This option is perfect for early-stage decentralized applications.

- Access to 50+ chains
- Rate limit: 200 requests/sec
- Pay-per-use options available

[Dedicated nodes](https://getblock.io/dedicated-nodes/) as a private service hosted by GetBlock guarantee simple integration of Web3 development solutions and seamless launching of all kinds of dApps. Endpoints for dedicated nodes are not charged from the account balance.

- No rate limits (1000+ requests/sec depending on a blockchain)
- 99.9% availability
- Custom settings

Select an API interface you want to use to interact with the blockchain in the dropdown next to each endpoint. Several API interfaces (JSON-RPC, REST, WS, etc) are available depending on the protocol.

![screenshot 3](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_3.webp)

## Step 4. Create shared node or dedicated node endpoints

Sign in to your account. You will see a basic dashboard with your endpoints and general statistics.
With your GetBlock account, you can create an unlimited number of endpoints for your shared nodes and dedicated nodes.

1. To create a [shared node](https://getblock.io/nodes/) endpoints, navigate to ‘Dashboard’ and scroll down to ‘My Endpoints’ section. Select a protocol, the network, and a desired API. Add as many access tokens to this protocol as you need. Your balance of requests for shared nodes is distributed on all projects marked with the ticker ‘Shared nodes’.
2. To create a [dedicated node](https://getblock.io/dedicated-nodes/) endpoint, switch over to the ‘Dedicated Nodes’ tab. Select a protocol and an available network. Click on ‘Get’ to proceed with configuring a dedicated node from the window that pops up. You can add more dedicated nodes following these steps. Add as many access tokens for each dedicated node as you need.

![screenshot 4](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_4.webp)

Next to each protocol or dedicated node, you will find an associated configuration file. Expand the endpoint to see all the access tokens generated for the protocol.

## Step 5. Get to know request packages for shared nodes

GetBlock offers various blockchain services, including access to nodes of 50+ leading networks.

Head to the 'Add Requests' tab in the sidebar to find the available pricing plans. The free plan includes a daily limit of 40,000 requests per account. Unused requests cannot be transferred to the next day and are, therefore, lost.

When your application is accessing a certain blockchain (sends tokens, verifies network states, etc.) it is called a ‘request’. You can choose between the ‘Pay Per Request’ and ‘Unlimited Access’ options.

With the pay-per-use option, purchased requests do not burn even if not used in 30 days.

Here is the calculation that helps to determine the time during which the whole amount of requests from the ‘Pay Per Request’ package will be spent at a maximum capacity set to 60 requests per second (RpS):

- 5,000,000 requests / (200 RpS * 60 sec) = 416 min (or 6 hrs 57 min);
- 10,000,000 requests / (200 RpS * 60 sec) = 833 min (or 13 hrs 53 min);
- 50,000,000 requests / (200 RpS * 60 sec) = 4166 min (or 69 hrs 27 min).

The ‘Unlimited’ plan users are given access to an infinite number of requests on all shared nodes for 1, 6, or 12 months.

![screenshot 5](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_5.webp)

To interact with shared nodes, select the required protocol and network, click ‘Get’, and receive your endpoint link in a matter of a few seconds.

Note that your balance of requests for shared nodes is distributed on all endpoints added under the ‘Shared nodes’ tab.

Additionally, you can increase your custom rate limit for shared nodes using the ‘Boost’ button found on the dashboard. Once approved, the limit will be applied to all shared endpoints. Contact our support team for more information.

## Step 6. Configure a dedicated node

You can configure a dedicated node by following an easy step-by-step process, which starts with selecting a protocol you want to deploy:

![screenshot 6](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_6.webp)

All you have to do next is choose a plan (an available discount is applied automatically) and set up your privately tailored API endpoint.

Pay for your dedicated nodes via the GetBlock account or select a customer support option if necessary.

## Step 7. Study GetBlock documentation

![screenshot 7](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_7.webp)

Dive deeper into [how GetBlock works](https://getblock.io/docs/), which methods it uses and how the blockchain node provider interacts with the nodes.

## Step 8. Creating a request to a node

To get connected to the blockchain node, copy an endpoint that includes an access token from your dashboard or retrieve the config file and import it into your App.

Ensure the secure storage of your access tokens. If compromised, an access token can easily be rolled or deleted. Press the '...' button next to the compromised endpoint and select the desired option.

You have the option to download configuration files for each protocol individually. These files will include all your access tokens for a specific endpoint in both JSON and JS formats. To obtain all the access tokens in one go, simply click the file icon next to 'My Endpoints.'

You can set up multiple access tokens for a selected blockchain or dedicated node if needed.

![screenshot 8](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_8.webp)

You can also download the Postman GetBlock’s [collection](https://documenter.getpostman.com/view/28751185/2s9YRDzqcX#ca02e504-8079-48e2-9bf0-d0a022b43774) to test our service.

![screenshot 9](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_9.webp)

Once the connection is established, the user can check the history of their requests.

Additionally, the user can access their connection with the command line interface (CLI). For instance, here’s how the height of the Binance Smart Chain (BSC) mainnet is verified by GetBlock CLI.

![screenshot 10](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_10.webp)

## Step 9. Checking the requests statistics

To check the statistics, head to the ‘My Endpoints’ section and switch to the ‘Statistics’ tab. You can customize the data view by parameters or by token using the dropdown menu.

Select the time period, a blockchain name, networks, and APIs to analyze the data.

![screenshot 11](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_11.webp)

All the information on the number of requests, response status, method calls, and rate limits rejection will be displayed in the form of infographics.

Stay tuned for more updates and announcements directly from GetBlock’s team.
