# What We Learned from Acala’s Extreme Testing Simulation

## Acala’s 3-week testnet campaign has concluded, highlighting the importance of a Canary Network and leading to several technical improvements to the network

![Image for post](https://miro.medium.com/max/1600/1*lGVbzGOgp5M3DqCPtAds8A.jpeg)

By: [Bette Chen](https://medium.com/u/8d475d21e811?source=post_page-----5ef5769a0902--------------------------------)

The Acala [Mandala Fest Season #3](https://medium.com/acalanetwork/acala-mandala-festival-season-3-d0a6f155c154), a 3-week testnet campaign, was successfully concluded on the 17th of August. It was a great way for us to demonstrate our development progress to the community by testing the system and protocols under heavy loads and extreme situations while providing rewards to participants.

We have been overwhelmed by the support, enthusiasm, and participation from the community. Here are some of the stats we have seen:

✅ 14,500 + new accounts

⛓️ 140,000 + meaningful transactions

💰 $52 million locked total value

💲 $25 million aUSD issued

**Award highlights are as follows and full results published** [**here**](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#season-3-prize-giving)**.**

😎 Week 1 awards went to 2,105 users out of 10,525 qualified

[⌛](https://emojipedia.org/hourglass-done/) Week 2 awards went to top 10 traders with an average return of 24,200%

🌋 Week 3 awards went to 200 users

✍️ 10 bloggers/vloggers awarded

🐞 45 bug hunters awarded

🤖️ 1 code bounty awarded

We have also learned some valuable lessons, some of which reaffirmed our preconceptions while others have led to improvements.

# The Importance of a Canary Network

Traditional blockchain development consists of only testnets and full production environments. However, we believe a blockchain cannot be properly tested without real economic conditions. From the Mandala testnet campaign, it is evident that with sporadic rewards (mostly via lucky draws for participants), while functionalities and usability to a large extend can be tested, the economic dynamics, liquidity efficiencies, and risk tolerance cannot be fully explored in a no-value testnet like Mandala.

Similar to Polkadot’s canary network [Kusama](http://kusama.network), Acala has implemented the [Karura](https://github.com/AcalaNetwork/Acala/wiki/1.-Get-Started#acala-trilogy-networks) canary network. Both networks bear real economic value, but a lower than that of the primary network (Acala in our case). Karura Network has economic value represented as its [KAR](https://github.com/AcalaNetwork/Acala/wiki/V.-ACA-&-KAR) native network token; it will be launched as parachain on the Kusuma network and provide financial primitives to the Kusama ecosystem such as accepting KSM as collateral for stablecoin credit lines.

# Lessons from Black Thursday Simulation — Liquidity is King

We may now have come to the realization that the financial risk tolerance of a decentralized (blockchain-based) financial system is by and large determined by the capacity and technical constraints of the underlying ledger. We have outlined the fundamental issues that led to MakerDAO’s 12th March Black Thursday incident [here](https://medium.com/acalanetwork/regaining-confidence-in-decentralized-stablecoins-bd98ba8e3c83):

- The performance bottleneck of the underlying network
- The ineffectiveness in liquidating risky collateralized loans or CDPs
- The inefficiency of keepers & liquidity crunch

## We have implemented the following improvements:

- **Quality of Service for oracle operations:** oracle transactions are prioritized and are always included in the block so price feeds are up-to-date and not affected by network traffic
- **Auto liquidator** using [Off-chain Workers](https://www.parity.io/substrate-off-chain-workers-secure-and-efficient-computing-intensive-tasks/): external actors like Keepers are required in protocols like Maker only because Ethereum or similar technology cannot provide a safe and secure auto-scheduler on a blockchain node. Acala implemented an auto-liquidator that can efficiently assess loan positions in every block.
- **Hybrid liquidation mechanism with DEX and auction:** the system will automatically liquidate collaterals on the DEX if price and slippage are favorable, to avoid price inefficiencies on auctions.
- **High throughput and specialization:** Acala has unoptimized throughput of 1000 tps; in Polkadot’s multi-chain universe, each shard/parachain is likely to be optimized for its use case. For example, Acala will be the financial shard optimized for DeFi operations, while another chain might specialize in gaming or breeding cats. The real throughput of Polkadot would be 1000 tps multiplied by the total number of shards/parachains connected.

During the campaign, Acala ran a Black Thursday drill to simulate severe price volatility resulting in liquidation of risky loan positions, followed by a system Emergency Shutdown. While under heavy load, the system performed as expected, and eventually all loans were processed and collaterals were returned to users.

📉 14,400+ loans were liquidated

⚡️ $1.37 million of assets were liquidated

# The Power of Cross-chain Liquidity

Acala is the finance hub of Polkadot’s multi-chain universe. It provides a suite of financial primitives including a multi-collateralized stablecoin, trustless staking derivative, and a decentralized exchange. These primitives are offered via Acala’s DApp directly to the end-users and also as SDKs for more DApps to be built upon. We see a more interconnected, autonomous, sophisticated, cross-blockchain finance ecosystem on the cusp of emergence.

We have integrated with Ren and Laminar and showcased the power of cross-chain liquidity:

₿ 1,403 renBTC was minted

👨‍🌾 $1.4 million worth of renBTC traded on DeX, $5.5 million used in lending

🌈 $4.3 million aUSD crossed to Laminar for synthetic asset (forex, gold, synthetic BTC & ETH) margin trading

Learn more about Acala cross-chain DeFi use cases [here](https://github.com/AcalaNetwork/Acala/wiki/T.-Cross-chain-DeFi); come and create the next killer DeFi project using our framework, DeFi primitives and SDKs. Our offerings are production-grade and production-ready. We were also an educational partner in Kusama’s recent Hackusama event, and you can learn more about building with Acala [here](https://medium.com/acalanetwork/hackusama-ea1ddf3e945a).

# Join Us

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launch, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).
