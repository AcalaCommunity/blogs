# Аудит безопасности Acala

![Image for post](https://miro.medium.com/max/8000/1*yhydywHe1k2421hd6xqhFQ.jpeg)

Мы в Acala считаем, что контроль над средствами пользователей должен быть, непосредственно, у самих пользователей, а не в руках корпораций. Нашей миссией является всячески развивать и поддерживать все финансовые приложения Web 3.0 - по-настоящему децентрализованной сети. В наших планах создать более открытое и честное финансовое будущее. Это будет возможно при помощи нашей, оптимизированной под DeFi, платформе смарт-контрактов и наших протоколов - децентрализованного стейблкоина, ликвидного стейкинга и DEX.

При этом, безопасность самого блокчейна Acala и протоколов является нашей приоритетной задачей. Мы приложили много усилий для разработки платформы и связанных с ней протоколов, которые, по нашему мнению, являются безопасными и надежными. Также, нами были привлечены лучшие специалисты для аудита нашего кода, среди которых: SRLabs, Trail of Bits и Slow Mist.

![Image for post](https://miro.medium.com/max/1730/1*hKvzkJVXDmSA9OU7NhFLuA.jpeg)

Аудиторская проверка была совершена в отношении модуля экосистемы RenVM, поддерживаемых сообществом модулей ORML, от которых зависит сеть Acala, а также внешнего интерфейса для DApp. На данный момент SRLabs и Slow Mist завершили свои аудиты, а вот проверка от Trail of Bits запланирована на январь 2021 года.

# Аудиторские заключения SlowMist и SRLabs

В ходе аудиторской проверки от SRLabs было обнаружено 0 критических ошибок, 1 высокую, 7 средних и 2 проблемы низкого уровня.

В ходе проведения аудита компанией SlowMist было обнаружено 0 критических, 0 высоких, 1 средняя и 1 проблема низкого уровня.

Единственная проблема высокого уровня, найденная во время аудита, была обнаружена нашей командой ещё до самого аудита и с того момента находится в процессе решения. We have now completed benchmarking and finalized appropriate weights for all [extrinsic](https://substrate.dev/docs/en/knowledgebase/learn-substrate/extrinsics) (aka signed/unsigned transactions, and inherits — info included in a block but not gossiped).

All other network security related issues have been addressed and reviewed by the auditors. There are two application-related issues (#5 and #8 in SRLabs report) are general DeFi issues such as DeX front-running, which yet to have a satisfactory solution. We are addressing it from a risk management perspective by setting safe parameters. Beyond that, we are seeking further economic audits that use simulation-based market stress testing so that we can evaluate vulnerabilities and market risks at a scaled volume and value.

The full report from SRLabs and SlowMist are [here](https://github.com/AcalaNetwork/Acala/tree/master/audit)

# Moving Forward

Audits are only one part of our effort in ensuring security and managing risks. All of Acala’s runtime codebases are audited, and upon genesis, all balances and governance decisions will be publicly verifiable. Our [Bug Bounty Program](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#runtime-bug-bounty) is also an important part to keep our codebase secure, and we encourage developers to dig into our code and report vulnerabilities. We believe transparency, time, and value are the true tests for the security of a network and protocols; so please be vigilant and help us make Acala safer and more secure for everyone.

# Join Us

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launch, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot, making fast and easy to use financial applications available to everyone. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.
