# Build Acala: тестовая парачейн-сеть Polkadot Rococo, сотрудничество с Ren, тестнет Mandala-мания, на The Defiant | Август 2020

Июль стал месяцем совместной работы с такими коллегами по экосистеме, как [ Ren ](https://renproject.io/) и [ Laminar ](http://laminar.one/), стресс-тестирование сети с десятками тысяч новых учетных записей и транзакций на протяжении всего Mandala Festival Season #3 и подготовка к запуску в тестовой парачейн-сети Polkadot Rococo.

![Image for post](https://miro.medium.com/max/8000/1*6wJEyP0ojcA8zM3SZAPzqQ.jpeg)

# **Обновления в девелопмент-сфере**

- ** Тестовая парачейн-сеть Polkadot ** [ ** Rococo: ** была запущена ](https://polkadot.network/introducing-rococo-polkadots-parachain-testnet/) ранее на этой неделе, что стало значительным шагом на пути к межсетевой интеграции. Парачейны теперь могут подключаться к релейной цепи, чтобы использовать ее общую безопасность, также доступна долгожданная передача сообщений между цепями, хотя она ограничена горизонтальной передачей сообщений, где релейная цепь будет использоваться для маршрутизации сообщений между двумя парачейнами. Acala работает над регистрацией на Rococo, чтобы проверить функциональность.
- [** Модуль RenVM-bridge **](https://github.com/AcalaNetwork/Acala/tree/master/ecosystem-modules) **и Интеграция renBTC: ** была развернута в тестовой сети Acala Mandala TC4, что стало первым шагом по внедрению renBTC в Acala и экосистему Polkadot. renBTC is now a fee token, can be used as collateral for stablecoin credit line, and is listed on Acala DeX.
- **Substrate RC4**: Mandala TC4 is now upgraded to [Substrate RC4](https://github.com/paritytech/substrate/releases/tag/v2.0.0-rc4), which allows atomic transactions — one step closer to production-ready smart contracts, and will soon be upgraded to the latest TC5 upon testnet campaign conclusion.
- **Acala Pulse**: an analytics dashboard to track stats of the network is under construction and will be released in the coming week. Users can track system fundamentals — aUSD issuance, DeX volume, and DOT amount in liquid staking, as well as system risks, liquidations and auctions, etc.
- **Black Thursday drill & Emergency Shutdown**: next week, [as part of the Mandala Festival](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#week-3-black-thursday-simulation), we will simulate Black Thursday volatility, test the hybrid liquidation mechanism that involves DeX and auctions to efficiently recover the loans. Then we will enact the system Emergency Shutdown, process all outstanding loans, and have users reclaim their collaterals from a basket of assets. _Festival week 3 rules & rewards are_ [_here_](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#week-3-black-thursday-simulation)_._

  ![Image for post](https://miro.medium.com/max/2880/1*XQbgIIFPlzwrK8L1eXdKew.jpeg)

# **Ecosystem Update**

- [**Ren x Acala / Polkadot**](https://medium.com/acalanetwork/bringing-btc-to-polkadot-acala-x-ren-e7959855d5aa?source=collection_home---4------2-----------------------) **to** bring Bitcoin and in future other isolated asset classes onto Acala and into the wider Polkadot multi-chain universe.
- [**Mandala Festival Season #3**](https://medium.com/acalanetwork/acala-mandala-festival-season-3-d0a6f155c154?source=collection_home---4------1-----------------------): started on two weeks ago, has generated quite a buzz with **_100k+ transactions, 13k new accounts, $2.5+ million aUSD issued from collateralizing renBTC, and 250+ (testnet) renBTC minted_**. Check [activities on Subscan](https://acala-testnet.subscan.io/).
- [**Hackusama with Acala**](https://medium.com/acalanetwork/hackusama-ea1ddf3e945a): Acala is an education partner for Hackusama, providing all of its runtime pallets and [common libraries](https://github.com/open-web3-stack/open-runtime-module-library) such as oracle and multi-token pallet, technical support and advice to the teams building DeFi projects.
- **Acala Foundation is now a council member** on Polkadot actively participating in Polkadot Direction riot discussion and voting. We appreciate your continued support so we can grow Polkadot and DeFi together 🚀

# **Events Update**

- **Unitize SF Blockchain Week**: Bette Chen co-founder of Acala talked about cross-chain DeFi in action. Watch [replay](https://next.brella.io/events/unitize2020/schedule/156155).
- **The Defiant**: Ruitao Su and Bette Chen chatted with Camila Russo on Polkadot being layer 0, how the ecosystem is evolving to have many domain-specific chain verticals and more. Podcast [here](https://anchor.fm/camila-russo/episodes/Developers-Will-Wake-Up-to-the-Fact-That-Theres-a-Toolkit-to-Build-Full-Fledged-Customized-Chains-Acalas-Bette-Chen-eh7sp0/a-a2pmg6h) & read [more](https://twitter.com/DefiantNews/status/1287758518913765377?s=20).
- Bette Chen being the outlier on the **Outlier Venture panel — “Prophesying the Future of Oracles”** alongside MakerDAO, DIA, Set Protocol and Aave. See Bette chat about yield farming [here](https://twitter.com/OVioHQ/status/1290644606892343297?s=20) & watch the full panel [replay](https://www.crowdcast.io/e/prophesying-oracles).

# About Acala

[Acala](http://acala.network/) is a first-of-its-kind decentralized finance consortium with a vision to bring financial stability, liquidity and accessibility to the mainstream. **The Acala Network is a cross-chain finance hub for the Polkadot ecosystem** and beyond. It offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative and a decentralized exchange to unleash liquidity and power financial innovations. It is the go-to open platform for finance-oriented dApps to deploy to using smart contracts or built-in protocols with out-of-box cross-chain capabilities, security and financial optimizations.

# Join Us

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala launch, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

![Image for post](https://miro.medium.com/max/1500/0*1KozUmtgLB7qV79q.jpeg)

Acala is a proud Web3 Foundation Grantee
