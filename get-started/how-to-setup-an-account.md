---
lastUpdated: June 10, 2023
---

# How to set up an account

To start using the GetBlock node connection services for building a decentralized application (dApp), an account should be registered and customized. It only takes a few clicks!

## Step 1. Signing up to GetBlock

Please, select a preferred sign-up option:

1. Connect wallet. By choosing this option, you are not required to share your email address and create a new password. If you do not currently have a wallet browser extension, you will be asked to install the extension.

2. Sign in with Google. Google will share your name, email address, language preference, and profile picture with getblock.io.

3. Sign up with email. You will be asked to provide your name and email address. Should you choose the first option, you’ll be asked to verify the email address you entered.

Note that to start using our service you will be asked to accept our [Terms of Service](https://getblock.io/terms-of-service/) and [Privacy Policy](https://getblock.io/privacy-policy/).

![screenshot 1](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_1.webp)

## Step 2. Check your user ID.

Find your user ID located in the ‘Account Settings’ section. Please use it when contacting GetBlock’s team so we can identify your account and help you faster.

![screenshot 2](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_2.webp)

## Step 3. Choose your way to interact with blockchain

With [shared nodes](https://getblock.io/nodes/), users can access peer-shared node infrastructure. This option is perfect for early-stage decentralized applications.

- Access to 50+ chains
- Rate limit: 60 requests/sec
- Pay-per-use options available

[Dedicated nodes](https://getblock.io/dedicated-nodes/) as a private service hosted by GetBlock guarantee simple integration of Web3 development solutions and seamless launching of all kinds of dApps. Endpoints for dedicated nodes are not charged from the account balance.

- No rate limits (1000+ requests/sec depending on a blockchain)
- 99.9% availability
- Custom settings

Select an API interface you want to use to interact with the blockchain in the dropdown next to each endpoint. Several API interfaces (JSON-RPC, REST, WS, etc) are available depending on the protocol.

![screenshot 3](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_3.webp)

## Step 4. Create shared nodes or dedicated nodes projects

Sign in to your account. You will see a basic dashboard with your projects. Each project displays a unique API key, which can be found in the top right corner.

With your GetBlock account, you can create an unlimited number of projects for your shared nodes and dedicated nodes. Please, note that one project can not be used for both shared and dedicated nodes:

1. To create a [shared nodes](https://getblock.io/nodes/) project, press the ‘+’ button in the ‘My projects’ section. Add as many shared endpoints to this project as you need. Your balance of requests for shared nodes is distributed on all projects marked with the ticker ‘Shared nodes’.
2. To create a [dedicated nodes](https://getblock.io/dedicated-nodes/) project, configure a dedicated node and select ‘create new’' when choosing a project. The project will be created right after your first dedicated node is deployed. You can add more dedicated nodes to the project later.

![screenshot 4](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_4.webp)

## Step 5. Get to know request packages for shared nodes

GetBlock offers various blockchain services, including access to nodes of 50+ leading networks.

In the ‘Account settings’ section, you will find available pricing plans. The free plan includes a daily limit of 40,000 requests per account. Unused requests cannot be transferred to the next day and are, therefore, lost.

When your application is accessing a certain blockchain (sends tokens, verifies network states, etc.) it is called a ‘request’. You can choose between ‘Launch’, ‘Build’, ‘Scale’, and ‘Unlimited’ options.

‘Launch’, ‘Build’, and ‘Scale’ plans are pay-per-use options. Purchased requests do not burn even if not used in 30 days.

Here is the calculation that helps to determine the time during which the whole amount of requests from a particular package will be spent at a maximum capacity set to 60 requests per second (RpS):

- **‘Launch’ pack**: 5 000 000 requests / (60 RpS * 60 sec) = 1 388 min (or 23 hrs 8 min);

- **‘Build’ pack**: 10 000 000 requests / (60 RpS * 60 sec) = 2 777 min (or 46 hrs 17 min);

- **‘Scale’ pack**: 50 000 000 requests / (60 RpS * 60 sec) = 13 888 min (or 9 days 15 hrs 28 min).

With the ‘Unlimited’ plan, users are given access to an unlimited number of requests on all shared nodes for 30 days.

![screenshot 5](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_5.webp)

To interact with shared nodes, select the required protocol and network, click ‘Get’, and receive your endpoint link in a matter of a few seconds.

Note that your balance of requests for shared nodes is distributed on all projects marked with the ticker ‘Shared nodes’.

You can set your custom requests limit for each project using the ‘Requests limit’ button. The limit will be applied to all endpoints within the project.

## Step 6. Configure a dedicated node

You can configure a dedicated node by following an easy step-by-step process, which starts with selecting a protocol you want to deploy:

![screenshot 6](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_6.webp)

All you have to do next is choose a plan (an available discount is applied automatically) and set up your privately tailored API endpoint.

Pay for your dedicated nodes via the GetBlock account or select a customer support option if necessary.

## Step 7. Study GetBlock documentation

![screenshot 7](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_7.webp)

Dive deeper into [how GetBlock works](https://getblock.io/docs/), which methods it uses and how the blockchain node provider interacts with the nodes.

## Step 8. Creating a request to a node

To get connected to the blockchain node, retrieve the endpoint from your account and insert it into your App. Each endpoint contains your project’s API Key. Please make sure to pass your API key in the path. You can also pass your API key in the header; if needed.

**Make sure that your API Keys are stored safely.**

![screenshot 8](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_8.webp)

You can also download the Postman GetBlock’s [collection](https://documenter.getpostman.com/view/12951625/TWDTNKP9) to test our service. Find the required node name and insert the API key.

![screenshot 9](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_9.webp)

Once the connection is established, the user can check the history of his/her requests.

Additionally, the user can access his/her connection with the command line interface (CLI). For instance, here’s how the height of the Binance Smart Chain (BSC) mainnet is verified by GetBlock CLI.

![screenshot 10](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_10.webp)

## Step 9. Checking the requests statistics

To check the statistics, select the blockchain name and the exact time period to analyze the data.

![screenshot 11](https://storage.getblock.io/web/docs/get-started/how-to-setup-account/screenshot_11.webp)

All requests will be displayed. If you are using multiple nodes, the information is also available in the form of infographics separately.

Stay tuned for more updates and announcements directly from GetBlock’s team.
