# Acala’s Decentralized Sovereign Wealth Fund — A Next-gen DAO & Unforkable AUM

By [Joe Petrowski](https://medium.com/u/9f4b86fbf09a?source=post_page-----80f8c23d8f27--------------------------------) & [Bette Chen](https://medium.com/u/8d475d21e811?source=post_page-----80f8c23d8f27--------------------------------)

**TLDR:** Acala is a next-generation DAO — DAO3.0 obtaining economic and political (decision making) sovereignty via its on-chain decentralized Sovereign Wealth Fund (dSWF) and governance. The assets in the dSWF are essentially Asset Under Management — while you can fork the code, the liquidity, and even the community, you cannot fork the AUM.

![Image for post](https://miro.medium.com/max/1600/1*tG3vPiETDyoJgt1aC_5ygg.jpeg)

Polkadot and Substrate provide the basis for new forms of societal organization and decision making. Acala is harnessing Substrate’s governance and treasury management capabilities along with Polkadot’s cross-chain messaging to create a decentralized sovereign wealth fund. The fund will enable the Acala chain to secure a parachain slot and continue development well after any initial fundraising runs out.

Before going into the mechanics of a decentralized sovereign wealth fund, let’s first discuss the traditional meaning. Like many open finance components, the decentralized variant has its roots in traditional finance.

High export countries often form sovereign wealth funds to manage their surplus and currency imbalances. When a country exports its goods, it receives foreign currency, like U.S. dollars, because the consumers purchase in their (the consumers’) local currency. But the exporting country needs to pay their own workers in their (the workers’) local currency. They typically have two options: sell USD and buy their own currency on the open market, or print more of their own currency. For central bankers and government officials, the former is not so desirable: It increases the value of their own currency relative to the currency it receives, therefore diminishing the value of future revenue. They may use a combination of both options, but will want to minimize the conversion of the foreign currency to their local currency. So what can they do with the excess? Sovereign wealth funds are state funds that often have a collection of foreign currencies as well as other assets like precious metals, equities, bonds, and real estate. Say what you will about Wall Street billions, even a mid-sized sovereign wealth fund makes the entire hedge fund industry look like a mom and pop shop.

A government run investment fund seems ripe for corruption and licentious lawmakers. That said, some sovereign wealth funds provide real value to their citizens; Norway’s, valued at over a trillion dollars, provides a pension for every citizen.

A decentralized sovereign wealth fund would provide a vehicle to deliver value to its citizens, but with the transparency and strict adherence to formal logic that blockchain allows. It could even go further. A typical wealth fund only serves to increase in value, but in a network where many tokens have _utility_, it could also gain access to functionality in other blockchain networks based on its holdings.

# Blockchains as Sovereign Entities

This topic all revolves around a central notion, that a blockchain can be a sovereign entity. Sovereignty implies a form of agency, decision making ability, and the power to exercise it. While sub-entities in blockchains like smart contracts have limited agency, a blockchain itself has not had agency or sovereignty. For example, with “Bitcoin on Ethereum”, a contract on Ethereum can own some Bitcoin, but Ethereum qua network cannot.

Substrate’s governance primitives allow chain builders to make sophisticated governance systems that involve general token holder voting as well as on-chain collectives with special management privileges. Besides the abstract decision making capabilities, Substrate can autonomously execute the results of governance decisions — including the decision to upgrade the chain itself.

The autonomous execution step is the fundamental element that allows Substrate-based chains to be sovereign. The chain enforces the will of its stakeholders and does not rely on miners, validators, etc. to participate in a hard fork. Polkadot allows its parachains to exercise full sovereignty and manage their governance independently. As such, every parachain in Polkadot, and the Relay Chain itself, can be considered sovereign entities with their own stakeholders.

Acala actually uses several on-chain councils, like a general council, a technical council, and councils to govern its sub-protocols Homa and Honzon. The general council — completely elected by token holders — manages its decentralized sovereign wealth fund. Because all the management is on-chain, token holders will have full insight into the fund’s management and can vote to replace general councillors.

# Fund Operation

The fund itself is represented by an on-chain account. This account does not have a private key associated with it. Instead, the general council and network governance have the capacity to manage the funds in the account.

Funds go into the account in three ways. The first two come from Acala’s Honzon protocol, which works similar to Maker. Honzon provides a multi-collateral lending platform that accepts several forms of collateral in exchange for a loan of aUSD, Acala’s stablecoin that is pegged to the US dollar. Just like in Maker, borrowers need to pay a stability fee on their loan. Unlike in Maker, instead of burning the fee, Acala deposits the fees into its sovereign wealth fund.

Second, the Acala network takes a penalty fee in case a loan’s collateral drops below some threshold. This fee prevents undercollateralized loans and only applies when the network needs to liquidate some collateral. Just like the stability fee, though, it goes into the wealth fund rather than being burned.

Third, Acala also operates a liquid staking protocol called Homa. Homa deserves an entire article on its own, but like the lending platform it should be nutshelled here. Polkadot, like other Proof of Stake networks, locks tokens to back validators and secure the network. If all goes well, those tokens make some return, but if the chosen validators misbehave, the tokens are liable for slashing. This schema is very much aligned with network security, but very much at odds with Acala’s thesis that funds should be able to serve contemporaneous purposes. Homa reconciles this tension by creating a staking pool where users can deposit DOT in return for some freely transferable L-DOT (although not necessarily at a one-to-one ratio). The pool is managed by the Homa Council for decisions like a validator selection strategy (again, whole other article), and L-DOT holders can return their L-DOT to the network and reclaim the underlying DOT plus its share of the staking revenue from the pool and minus some fee that goes — you guessed it — into the sovereign wealth fund.

A large proportion of revenue comes from sources where other protocols would have burned tokens. Many protocols burn tokens as a mechanism of making everyone’s tokens more valuable by reducing the total issuance. Burning tokens, however, does not _create_ value, it only reallocates existing value. By moving the value into a collective fund, the network will use the funds to drive value creating relationships.

# Value Creation

Just creating this fund is amazing in its own right. This single account actually owns multiple currencies not just from within its own blockchain, but from other blockchains as well. And this account doesn’t represent a contract or any user or business or entity: it is actually owned by the chain itself. Pause and think about that for a moment. The chain didn’t assign a foreign chain asset to a user or contract; rather, one blockchain (Acala, in this case) has a stake in another blockchain.

Currencies and tokens can serve many purposes, so the Acala stakeholders will decide how to use their funds. Acala first plans to use these funds to secure a parachain slot. Polkadot has a limited number of parachain slots, and when a new one becomes available, an auction where teams bid to lock DOT determines who can use it. Most teams won’t have enough DOT on their own to secure a slot and will resort to crowdfunding by asking users to lock their DOT on behalf of the project. Acala will do the same for its first parachain auction.

But crowdfunding the same project over multiple auctions is not sustainable. If the sovereign wealth fund can raise enough funds, the blockchain itself could secure its own parachain slot and return all previous crowdfunded DOT to the contributors.

When tokens enter this fund, Acala plans to convert them all to DOT and stake it behind validators in order to grow the fund from its three revenue streams by adding staking return on DOT. When its first parachain slot is up for its renewal auction, it will unstake the DOT and use it in its own crowdfunding. Eventually, it will have enough DOT to cover the parachain bond without resorting to crowdfunding.

After Acala has its own parachain slot, it can continue the sovereign wealth fund in pursuit of other utility. Rather than accumulating DOT for the singular goal of obtaining a parachain slot, it can take positions in other parachains for access to their services or partnerships.

The effects of blockchain sovereignty extend well beyond a chain’s own governance. By combining new advances in blockchain governance, interoperability, and economics, Acala has created an innovative and sustainable funding model for their future that puts the stakeholders in control of the chain’s destiny.

# Looking Ahead

Through the dSWF and governance, Acala will become an economic and political (decision making and execution) sovereign entity. It will pioneer a new way of DAO — DAO 3.0. Just like Norway’s Sovereign Wealth Fund, Acala’s dSWF will reinvest its network surplus in foreign assets — starting with DOT and KSM and gradually diversify into other assets, for the purpose of gaining access to network security, long term wealth generation, and strategically holding stakes in valuable sovereign networks. ACA holders not only collectively own the dSWF, but also can collectively decide how to deploy the dSWF. The funds in the dSWF are essentially the Assets Under Management (AUM) of the Acala network. You can fork the code, the liquidity, and even the community, but you cannot fork AUM.

More details in the [dSWF Whitepaper](https://github.com/AcalaNetwork/Acala-white-paper/blob/master/Building_a_Decentralized_Sovereign_Wealth_Fund.pdf).

# Join Us

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launch, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot, making fast and easy to use financial applications available to everyone. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.
