# Acala представляет смарт-контракты и совместимость с Ethereum для Polkadot DeFi

## Acala теперь поддерживает EVM и ink! паллеты на Substrate, что позволяет разработчикам использовать смарт-контракты на основе Solidity и Wasm

![Image for post](https://miro.medium.com/max/1600/0*-4rCl6SjqDKz7eBh)

Автор статьи: [Брайан Чен](https://medium.com/u/241f963260c9?source=post_page-----588b3891e53d--------------------------------)

Polkadot разработан как для простой интеграции с другими блокчейнами, такими как Bitcoin и Ethereum (через мосты, такие как Interlay и RenVM), так и для размещения ряда разнородных (так называемых независимых и настраиваемых), но взаимосвязанных цеей, называемых парачейнами. Polkadot больше похож на цепь инфраструктуры уровня 0, обеспечивая базовый уровень доверия, который поставляется с общей безопасностью Proof of Stake (PoS) и межсетевым взаимодействием. Цепи парачейнов, скорее всего, будут цепями для конкретной предметной области, оптимизированными для их вариантов использования и решения конкретных проблем предметной области, где Acala занимает сферу децентрализованных финансов. Мы предлагаем набор готовых примитивов DeFi, таких как стейблкоин (aUSD), деривативы для стекинга (например, позволяющие выкупить токены (LDOT) на застеканном/залоченном DOT) и децентрализованный обмен, чтобы обеспечить больше инноваций DeFi. Мы также создали общие служебные модули с открытым исходным кодом, такие как оракул, мультивалютную, универсальную среду мониторинга, которую могут использовать команды.

Парачейны на основе Substrate, такие как Acala, будут пользоваться полным технологическим стеком, предоставляемым этой структурой, начиная от технической инфраструктуры низкого уровня (RPC, среда выполнения веб-сборки, одноранговая связь и т. д.), до модулей уровня приложения, которые позволяют EVM (виртуальная машина Ethereum) и возможности смарт-контрактов. Это означает, что в обозримом будущем инновации на уровне цепи и технологический прогресс будут происходить с беспрецедентной скоростью и в больших масштабах; новые возможности будут легко и беспрепятственно реализованы в режиме plug-and-play с помощью безфорковых обновлений для всех цепей на основе Substrate (см. примеры на [рынке Substrate](https://marketplace-staging.substrate.dev/)).

Тем не менее, в Acala теперь доступны следующие возможности смарт-контрактов:

1.  Acala поддерживает паллет EVM (также известный как модуль времени выполнения), который, по сути, является реализацией виртуальной машины Ethereum на Substrate, так что контракты Solidity могут быть развернуты и запущены на Acala.
2.  Acala также поддерживает ink! контракт паллеты, которые позволяют использовать собственные смарт-контракты Substrate на основе Wasm (Web Assembly), написанные на Rust.

Это обновление обусловлено как техническим прогрессом, так и интересами сообщества. Acala помогает ряду протоколов, изучающих кросс-чейн развертывания DeFi на Polkadot, механизмы, о которых мы расскажем в этой статье, и смарт-контракты, безусловно, являются одним из важных направлений для изучения. В дальнейшем Acala будет более активно сотрудничать с [Parity](https://www.parity.io/) и другими участниками экосистемы, такими как [Moonbeam](https://moonbeam.network/), [Plasm](https://www.plasmnet.io/) и [Edgeware](https://edgewa.re/), и участие в разработке EVM и смарт-контрактов.

# Сейчас мы рассмотрим следующие темы:

1.  Кросс-чейн ликвидность через мосты
2.  Способы развертывания на Polkadot
3.  Способы развертывания на Kusama
4.  Способы развертывания на Acala
5.  Текущее состояние смарт-контрактов на Polkadot

# Кросс-чейн ликвидность через мосты

Мосты - это интероперабельная технология для передачи активов и сообщений между двумя экономически суверенными и технологически разными цепями, например между Polkadot и Ethereum или Bitcoin. Существуют разные виды мостов: от централизованных и надежных до более децентрализованных и ненадежных.

1.  **Кастодиальные решения**: при использовании типов настройки с несколькими подписями или Proof of Authority (PoA) их относительно проще реализовать и они доступны для использования прямо сейчас. [ChainX](https://chainx.org/) как Bitcoin мост и [ChainSafe](https://chainsafe.io/) как мост Ethereum являются примерами этого типа, а дорожные карты со временем станут более децентрализованными.
2.  **Решения без доверия**: использование экономических и/или криптографических гарантий для передачи активов в/из двух блокчейнов; они не вызывают доверия, но могут быть дорогостоящими для пользователей, а также все еще находятся в стадии исследований и разработок из-за технических проблем, связанных с ненадежной природой. [Interlay](https://medium.com/interlay/bitcoin-on-polkadot-proof-of-concept-for-trustless-bridge-shipped-6fb8e549bef0) как Bitcoin мост и [SnowFork](http://www.snowfork.com/) и [Darwinia](https://darwinia.network/) как мост Ethereum являются примерами этого типа.
3.  **Гибридные кастодиальные/надежные решения**: тогда есть решение [RenVM](https://renproject.io/), которое не требует прав доступа, с отличным пользовательским интерфейсом и популярностью с четким путем к децентрализации, но сейчас больше доверие было возложено на Команду Ren.

Acala нейтральна в отношении подходов к решениям мостов, поскольку разные типы мостов могут удовлетворять разные предпочтения пользователей в отношении надежности, удобства и стоимости, и есть веские причины для того, чтобы различные типы мостов сосуществовали и удовлетворяли различные потребности.

# Развертывание на релейной цепи Polkadot

Как уже упоминалось, Polkadot - это кросс-чейн инфраструктурная цепь 0-го уровня (называемая [Relay Chain](https://wiki.polkadot.network/docs/en/learn-architecture#relay-chain)). Applications and protocols hence cannot be deployed directly on the Relay Chain but rather via the following mechanisms provided as fabrics of the Polkadot network, each with its own trade-offs:

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
