# AcalaはPolkadot Testnetで最初のパラチェーンをローンチします

![投稿画像](https://miro.medium.com/max/8000/1*IGXwgFXEA7viM8upZgcw2g.jpeg)

AcalaをPolkadotのパラチェーンとしてローンチする為の重要なマイルストーンに到達しました。[Rococo - Polkadotのパラチェーンテストネット](https://medium.com/polkadot-network/introducing-rococo-polkadots-parachain-testnet-e3e67fc40b56)の最初のパラチェーンとしてAcala Mandala PC1 (Parachain Candidate 1) テストネットをローンチしました。

Rococo enables parachain consensus and shared security via [Cumulus](https://wiki.polkadot.network/docs/en/build-cumulus), as well as cross-chain communication via HRMP (Horizontal Relay-chain Message Passing). HRMP requires cross-chain messages being routed via Relay-chains, as a stepping stone towards direct parachain to parachain communication via [XCMP](https://wiki.polkadot.network/docs/en/learn-crosschain) (Cross-chain Message Passing) later on.

With Acala Mandala PC1, we can

- **Test Acala’s full DeFi suite** (stablecoin, staking derivative, and DeX) using cross-chain consensus and message passing.
- Develop further the [Cross-Consensus Message (XCM) format](https://github.com/paritytech/xcm-format) implementation, and specifically flesh out the **cross-chain fungible token standard** that we had spearheaded. The draft standard [here](https://github.com/w3f/PSPs/blob/master/PSPs/drafts/psp-3.md) & PoC pallet implementation [here](https://github.com/open-web3-stack/open-runtime-module-library/tree/rococo/xtokens).
- **Test Acala Collator nodes** and implement reward schemes.
- **Test cross-chain integrations** **with other parachains** such as Laminar, Plasm, Interlay, and others.
- Implement Homa protocol’s **trustless staking bridge to Relay-chain**.

# Parachain Developer Community

We have shared the following with the parachain developer community

- **Turn a Substrate-based chain into a parachain** including turning nodes into [Collators](https://wiki.polkadot.network/docs/en/maintain-collator) by integrating Cumulus [here](https://github.com/AcalaNetwork/Acala/pull/362)
- **Cross-chain fungible multi-token transfer implementation** — the ‘xtoken’ pallet [here](https://github.com/open-web3-stack/open-runtime-module-library/tree/rococo/xtokens). This already enables transferring ROC (Rococo’s network token) between Rococo and Mandala PC1; other parachains who adopt this or use the same standards can transfer tokens to each other.

# What’s Next

For the Mandala PC1, it will reset inadvertently unannounced multiple times to keep up with the latest version of Rococo, roll out new functionalities and support integrations with other parachains. The key upcoming developments for the Mandala Parachain Candidate are:

- **Continue to develop the XCM pallet** along with Parity, the Web3 Foundation, and others in the community towards production-ready.
- **Enable Acala staking** with rewards/slash on Acala Collator nodes.
- **Extensive cross-chain communication testing** with other parachains, and make possible some of the use cases that were implemented in isolation, for example, and cross aUSD to Laminar as the base currency for margin trading, and cross aUSD to Plasm network as payment methods.
- **Enable Homa staking derivative (LDOT) Relay-chain bridge** so that trustless liquid staking for Kusama and Polkadot is ready on launch.

# Launch

Beyond Rococo and Mandala, Acala will launch its canary network Karura as parachain firstly on Kusama when parachain function is enabled there, then launch mainnet on Polkadot. Acala will operate the two networks — Karura & Acala mainnet to provide DeFi infrastructure and liquidity for both Kusama and Polkadot ecosystem. From here on, we will be preparing for parachain auction to secure a slot and launch on the two networks. **Subscribe** [**here**](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) **to receive updates on the Acala parachain auction and launch.**

# About Acala

[Acala](http://acala.network/) is a first-of-its-kind decentralized finance consortium with a vision to bring financial stability, liquidity and accessibility to the mainstream. The Acala Network is a cross-chain finance hub for the Polkadot ecosystem and beyond. It offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative and a decentralized exchange to unleash liquidity and power financial innovations. It is the go-to open platform for finance-oriented dApps to deploy to using smart contracts or built-in protocols with out-of-box cross-chain capabilities, security and financial optimizations.

**Join Us**

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

![Image for post](https://miro.medium.com/max/1500/0*YTeYSsHAVjOBCZu8.jpeg)

Acala is a proud Web3 Foundation Grantee
