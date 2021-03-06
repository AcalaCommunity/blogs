# Acala Unveils Smart Contracts and Ethereum Compatibility for Polkadot DeFi

## Acala now supports the EVM and ink! pallets on Substrate, enabling Solidity and Wasm-based Smart Contracts for developers

![Image for post](https://miro.medium.com/max/1600/0*-4rCl6SjqDKz7eBh)

By: [Bryan Chen](https://medium.com/u/241f963260c9?source=post_page-----588b3891e53d--------------------------------)

Polkadot is designed both to easily integrate with other blockchains such as Bitcoin and Ethereum (via bridges like Interlay and RenVM), and to host a number of heterogeneous (aka independent and customizable) but interconnected chains, called parachains. Polkadot is more like a layer-0 infrastructure chain, providing the underlying trust layer that comes with shared Proof of Stake (PoS) security and cross-chain communication. The parachain chains are more likely to be domain-specific chains optimized for their use cases and solving specific domain problems, where Acala occupies the domain of decentralized finance. We offer a suite of out-of-the-box DeFi primitives such as a stablecoin (aUSD), staking derivatives (e.g. allowing you to redeem tokens (LDOT) on staked/locked DOT) and a decentralized exchange to power more DeFi innovation. We’ve also open-sourced common utility modules such as an oracle, multi-currency, generic monitoring framework for teams to use.

Substrate-based parachains like Acala will enjoy the full-tech-stack provided by this framework ranging from low-level technical infrastructure (RPC, web-assembly runtime, peer-2-peer communication etc.), to application-layer modules that enable EVM (Ethereum Virtual Machine) and Smart Contract capabilities. This means in the foreseeable future chain-level innovation and technological advancements will happen at an unprecedented speed with large scale; new capabilities will be plug-and-play via forkless upgrades across all Substrate-based chains easily and seamlessly (see examples on [Substrate marketplace](https://marketplace-staging.substrate.dev/)).

That said, Acala has now enabled Smart Contract capabilities in the following fashions:

1.  Acala supports the EVM pallet (aka runtime module), which is essentially an Ethereum Virtual Machine implementation on Substrate so that Solidity contracts can be deployed and run on Acala.
2.  Acala also supports the ink! contract pallet, which enables Wasm (Web Assembly) based Substrate native Smart Contracts written in Rust.

This update is driven by both technical progression and community interests. Acala is helping a number of protocols exploring cross-chain DeFi deployments on Polkadot, the mechanisms of which we will unpack in this article, and Smart Contracts is certainly one of the important avenues to explore. Hereafter Acala will be more actively collaborating with [Parity](https://www.parity.io/) and others in the ecosystem such as [Moonbeam](https://moonbeam.network/), [Plasm](https://www.plasmnet.io/) and [Edgeware](https://edgewa.re/), and contributing to the EVM and smart contract development.

# We will now go into depth on the following topics:

1.  Cross-chain Liquidity via Bridges
2.  Ways to deploy on Polkadot
3.  Ways to deploy on Kusama
4.  Ways to deploy on Acala
5.  The current state of Smart Contracts on Polkadot

# Cross-chain Liquidity via Bridges

Bridges are interoperable technology to cross assets and messages between two economically sovereign and technologically diverse chains e.g. between Polkadot and Ethereum or Bitcoin. There are different flavors of bridges ranging from centralized and trusted to more decentralized and trustless.

1.  **Custodial solutions**: using multi-sig or Proof of Authority (PoA) types of setup, they are relatively easier to implement and are available to use right now. [ChainX](https://chainx.org/) as Bitcoin bridge and [ChainSafe](https://chainsafe.io/) as Ethereum bridge are examples of this type, with roadmaps to become more decentralized over time.
2.  **Trustless solutions**: using economic and/or cryptographic guarantees to transfer assets to/from two blockchains; they are trustless, but could be expensive to users, and also are still under research and development due to technical challenges of its trustless nature. [Interlay](https://medium.com/interlay/bitcoin-on-polkadot-proof-of-concept-for-trustless-bridge-shipped-6fb8e549bef0) as a Bitcoin bridge and [SnowFork](http://www.snowfork.com/) and [Darwinia](https://darwinia.network/) as an Ethereum bridge are examples of this type.
3.  **Hybrid Custodial/Trustless solutions**: then there’s the [RenVM](https://renproject.io/) solution that is permissionless with great UX and popularity with a clear pathway towards decentralization, but right now much trust has been placed on the Ren team.

Acala is neutral with regards to approaches to bridge solutions, as different flavors of bridges may satisfy different user preferences of trustlessness, convenience and costs, and there are good reasons for various types of bridges to co-exist and serve various needs.

# Deploying on the Polkadot Relay Chain

As mentioned, Polkadot is a Layer-0 cross-chain infrastructure chain (called the [Relay Chain](https://wiki.polkadot.network/docs/en/learn-architecture#relay-chain)). Applications and protocols hence cannot be deployed directly on the Relay Chain but rather via the following mechanisms provided as fabrics of the Polkadot network, each with its own trade-offs:

1.  **Deploying as a parachain** — This option has the highest degree of customizability and flexibility both technically and economically. It has more ‘permanent’ access (within the parachain lease period) to Polkadot’s shared security and cross-chain communication facility. It does have a higher cost to set up, and require much more effort to bootstrap and maintain the network as well as the community. You can get a taste of this by [exploring Acala](https://github.com/AcalaNetwork/Acala/wiki/1.-Get-Started).
2.  **Deploying as a parathread** — it’s similar to parachain technically, but uses a pay-as-you-go model for security and communication access, hence less overhead upfront and cheaper to run. If a chain cannot get a parachain slot, it can fall-back to parathread to continue its operations.
3.  **Deploying as a DApp on an active parachain/parathread** — for teams who want to access the Polkadot ecosystem but don’t want to build and maintain a blockchain, or who want to try things out without much upfront commitment, then deploying on an existing parachain might be a good option. Especially for DeFi related DApps, you can treat Acala as a landing pad (such as in [Ren’s case](https://medium.com/acalanetwork/bringing-btc-to-polkadot-acala-x-ren-e7959855d5aa?source=collection_home---4------6-----------------------).) and a technical-know-how Polkadot-buddy when exploring the space.

Apart from technical and economic considerations, one shall also think of composability. The degree and sophistication of composability may vary depending on where you land — DApps on one parachain would naturally enjoy a higher degree of composability within that chain (read Ren’s integration [here](https://github.com/AcalaNetwork/Acala/wiki/T.-Cross-chain-DeFi#ren)), cross-parachain DApps may have reduced composability and atomicity of transactions (read Laminar’s integration [here](https://github.com/AcalaNetwork/Acala/wiki/T.-Cross-chain-DeFi#laminar)), and bridges may have even lower composability as they are mostly focused on value transfers and certain specific message passing across designated blockchains.

# Deploying on Kusama’s Relay Chain

[Kusama](http://kusama.network), similar to Polkadot, is a Layer-0 cross-chain infrastructure chain with a core [Relay Chain](https://wiki.polkadot.network/docs/en/learn-architecture#relay-chain) that provides security and interoperability. Kusama is meant to be a development environment for teams preparing for deployment on Polkadot, or for teams who want to build exclusively on Kusama for lower economic barriers to parachain slots and for faster governance cycles. Developers have the same options with Kusama as they do with Polkadot, with a few caveats:

1.  **Deploying as a parachain** — Teams can build a parachain on Kusama for three primary reasons. First, parachains can be deployed to Kusama after passing testing on the Westend testnet in order to fine-tune their technology before a full deployment to Polkadot. Some teams, Acala included, will choose to operate parachains on both Polkadot and Kusama to serve both communities. Third, teams (e.g. new startups) may also choose to stay exclusively on Kusama if the cost for a Polkadot parachain slot is out of reach or if they prefer the risk-taking and fast-moving nature of Kusama. The Kusama parachain option is also customizable and flexible both technically and economically.
2.  **Deploying as a parathread** — Kusama will have the same parathread functionality as Polkadot, which is a pay-as-you-go model for security and communication access, leading to less overhead and expense to run. One tradeoff is that parathreads come with less frequent block submissions to the Relay Chain, so it may suit some use cases better than others.
3.  **Deploying as a DApp on an active parachain/parathread** — DApps can be built on Kusama parachains or parathreads. DeFi DApps for example can be built on Acala’s Kusama Network, as well as many other use cases like gaming, communications, social media, or DAOs.

In the next sect we will explore different ways to deploy on Acala parachain.

# Deploying on the Acala Parachain

You can treat Acala as the DeFi landing pad on Polkadot and Kusama, and your technical-know-how builder-buddy. There are currently three ways you can deploy on Acala:

1.  **Deploy runtime modules (aka pallets)** — this enables the highest level of customizability, and access to Acala’s chain logic for a more sophisticated integration. It does not have the fail-safe sandbox environment that smart contracts enjoy, hence it requires security audits and requires governance permission. It suits better for infrastructure and common-good protocols. The [RenVM bridge module](https://github.com/AcalaNetwork/Acala/tree/master/ecosystem-modules/ren/renvm-bridge) is a good example of this. A brand new account with only freshly minted renBTC, can perform any transactions on Acala without needing a fee token. Thanks to Acala’s FlexFee feature, tokens like renBTC are integrated natively as one of the default fee tokens alongside ACA, aUSD and DOT.
2.  **Deploy Solidity smart contracts** — for those who want to migrate part or all of their existing Solidity smart contracts to Polkadot without re-writing all the code, this can be a good starting point. As an example, some teams would use a bridge to cross their tokens from Ethereum to Polkadot, then deploy on Acala for faster, cheaper transactions and better user experience.
3.  **Deploy ink! smart contracts** — this is Substrate’s native, Rust-based Wasm smart contract, read more on how it compares to EVM [here](https://substrate.dev/docs/en/knowledgebase/smart-contracts/ink-fundamentals).

As a disclaimer, smart contract modules are close to but not yet (to Acala’s standard) production-ready, and we will be working closely with Parity and others in the ecosystem to finalize them. We outline the caveats and current state of the development in the next section.

# The Current State of Smart Contracts

## EVM

While Solidity and EVM-compatible contracts can be deployed and run on Substrate-based chains like Acala, much of the tooling is still being developed so that it’s compatible with existing development tools such as Truffle and Remix etc. SDKs are also being developed to be compatible with existing web3.js and other libraries. Acala will also focus on improving the composability of smart contracts and runtime modules to accelerate cross-chain DeFi innovation.

## Ink! Smart Contracts

Rust-based ink! smart-contract language is still under development, as are its development tooling (cargo-contract and [Redspot](https://github.com/patractlabs/redspot) — Truffle for Ink!) and SDKs (polkadot.js).

# Next Steps

Acala now supports EVM with the [Frontier](https://github.com/paritytech/frontier) Substrate-Ethereum compatibility layer. We can now run unmodified Ethereum DApps. Next, we will be deploying more complex (real-life) Solidity contracts, testing out tooling supports including Metamasks, and implementing pallet (runtime module) integration to improve compatibility, and to become compatible with ERC20 and other token standards.

Consider this your official invitation to [**Build with Acala**](https://github.com/AcalaNetwork/Acala/wiki/U.-Build-with-Acala), where we support and help teams create valuable cross-chain DeFi projects with Polkadot and Kusama.

# Join Us

[Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launches on Polkadot and Kusama, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot that makes it fast and easy to use or build financial applications, improving trading efficiency and saving valuable time. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.
