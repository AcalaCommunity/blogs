# Introducing the Open Oracle Gateway for Polkadot

## The Open Oracle Gateway provides open, inclusive and progressively decentralized price oracle services to the ecosystem in Acala, Karura, Polkadot, Kusama and beyond.

By [Bette Chen](https://medium.com/u/8d475d21e811?source=post_page-----3554f7a4254e--------------------------------) and [Bryan Chen](https://medium.com/u/241f963260c9?source=post_page-----3554f7a4254e--------------------------------)

![Image for post](https://miro.medium.com/max/1600/0*oEYR17rjpn2J6bQN)

# Acala’s Previous Approach to Oracles

Up until now, Acala previously ran its own oracle network with multiple operator nodes sourcing off-chain data for on-chain operations such as evaluating borrowing capacity and liquidation risks. The Acala team has designed this infrastructure to meet the specific demands of DeFi applications through the following features:

- **Multiple Operators**: the Acala oracle provider network accepts data feeds from multiple nodes, and the aggregator combines the data to a single price to reduce attack factors.

- **Quality of Service**: Oracle operations are classified as high-priority transactions that will be included in a block regardless of network state (e.g. congested), so that price feeds are more reliable with minimum delay.

- **Customizable Fees**: the team implemented a favorable fee schedule (e.g. price feeds can be free) and DDoS attack protection, e.g. to allow 1 call per block from each authorized provider to ensure security and maintain cost-efficiency.

- **Progressive Decentralization**: Initially, oracle providers will be authorized and whitelisted to maximize security and predictability, while gradually shifting to be more permissionless and trustless over time.

With the current setup, other oracle providers can provide independent price feeds by running an operator node; however, it only supports one oracle network. The challenge of providing reliable, accurate and decentralized oracles cannot be solved by Acala alone. When taking into account that Acala is the DeFi hub and platform powering more cross-chain DeFi DApps on Polkadot, Kusama and beyond, creating a more open, inclusive, and decentralized oracle infrastructure with other leading projects in the industry becomes critical.

# Moving Forward — The Open Oracle Gateway

Today the Open Oracle Gateway, a technical collaboration between the Acala, Laminar and Band Protocol teams, is a significant step towards the vision of creating an open, inclusive, and decentralized oracle network for the Polkadot ecosystem. The Gateway offers the following:

# Multiple Oracle Networks

The Gateway allows multiple parties in addition to Acala to operate their own oracle networks and provide price feed services. Essentially any oracle service provider can set up a new Network Provider, and through governance approval, it would be enacted through runtime upgrade. Node Operators can then be set up for this new network and start posting off-chain data to Acala. These data feeds are aggregated into a single price feed available to consumption via the Gateway.

View the default oracle pallet (the Provider) [here](https://github.com/open-web3-stack/open-runtime-module-library/tree/master/oracle).

An oracle Network Provider can implement their own oracle pallets (based on the default oracle pallet) to meet their specific requirements such as validating cross-chain data feeds. We can also easily integrate with existing signed oracle APIs such as [Coinbase price oracle](https://blog.coinbase.com/introducing-the-coinbase-price-oracle-6d1ee22c7068) by simply adding a Coinbase Provider pallet and validate their signature.

The Gateway is essentially a meta-network/meta-aggregator of oracle networks/aggregators that will encourage an ecosystem of service providers to provide differentiated services to meet various needs of applications.

Acala network will progressively decentralize, and its governance will start with PoA (appointed Council governance), then evolve into elected Council governance, and eventually democracy. The implication for the Gateway is that initially the Network Providers and their respective node Operators will be known parties and be approved to join the Gateway by the sitting Council.

# Price Feeds by Choice

DApps can choose to use price feeds from one particular Provider based on their preferences. Alternatively, they can also choose to use an aggregated feed combining the data from all of these providers. DApps can also obtain raw data from individual node operators and aggregate them themselves. The aggregator can be further customized, so data consumers can choose to use a median price, an average or whatever methods they favor.

# Quality of Service & Free Feeds

All price feeds posting to Acala regardless of which provider network they belong to, will be provided with Quality of Service. Transactions submitted by the Operator are _operational transactions_ — system critical transactions that are prioritized and guaranteed to be included in a block. This will prevent invalid and out-of-date price feeds due to spikes in gas fees and congested networks, such as in the case of [Black Thursday](https://medium.com/aave/crypto-black-thursday-the-good-the-bad-and-the-ugly-7f2acebf2b83).

In addition, all _valid_ feeds will be refunded with the transaction fees incurred, essentially making oracle feeds FREE while preventing spam and ensuring integrity. A valid feed transaction would need to be signed and posted by an approved Operator, and only one transaction is permitted by the same Operator within a single block.

# Project Status & Next Steps

We hope the Open Oracle Gateway becomes a common good infrastructure for the Acala, Polkadot, Kusama and the cross-chain DeFi ecosystem in general. **With that said, we welcome any oracle service providers to check out the Gateway source code, talk to us about integration, contribute to the codebase and provide your services to an ever-growing ecosystem.**

An [example](https://acala-testnet.subscan.io/runtime/OperatorMembershipAcala?version=606) of a running Oracle network on Acala’s testnet.

An [example](https://acala-testnet.subscan.io/account/5Fe3jZRbKes6aeuQ6HkcTvQeNhkkRPTXBwmNkuAPoimGEv45) of the Acala Oracle Operator feeding prices on-chain.

The aggregated price feed is a calculated value that can be read via RPC calls using [acala.js](https://github.com/AcalaNetwork/acala.js).

Going forward, we may set up a separate Oracle Council to make on-chain decisions on Providers and their Operator membership and other related affairs. As we progressively decentralize the Acala network, the Gateway will also be further decentralized. With customizable chain logic and economic policies on the Acala chain, the design space for oracle economic models and on-chain payment mechanisms is huge and we are only scratching the surface.

# Get Involved in the Open Oracle Gateway

The Open Oracle Gateway itself is designed to be an infrastructure that anyone can extend and improve. **If you are a developer or oracle service provider, please check out** [**the Open Oracle Gateway Wiki**](https://wiki.acala.network/learn/basics/oracle)**, and join the discussion on** [**Discord**](https://discord.gg/jYC5QeG)**.**

_Interested in a career in decentralized finance? If you enjoy working on high-impact, web3 and DeFi challenges, check out_ [_our open positions_](https://jobs.lever.co/acala/) _here. We’d love to hear from you._

**This post was also published on the Polkadot blog here:**

[Introducing the Open Oracle Gateway for Polkadot](https://medium.com/polkadot-network/introducing-the-open-oracle-gateway-for-polkadot-1cf2e1b71c92)

# Join Acala’s Community

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)To keep up to date with progress on the Acala parachain launch, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot, making it fast and easy to use financial applications available to everyone. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de-facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.
