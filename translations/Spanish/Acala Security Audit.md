# Acala Security Audit

![Image for post](https://miro.medium.com/max/8000/1*yhydywHe1k2421hd6xqhFQ.jpeg)

At Acala we believe individual users, not corporations, should be in control of their own finance. Our mission is to support and nurture financial applications of Web 3.0 — the truly decentralized and “trustless” web. A more open and fair financial future is what we hope to enable through our DeFi-optimized Smart Contract platform and our protocols — decentralized stablecoin, trustless liquid staking and decentralized exchange.

That said, the security of Acala’s blockchain and protocols is our highest priority. We have invested considerable efforts to develop a platform and associated protocols that we believe are safe and reliable; we have also engaged the best in the business to help audit our codebase — amongst them are [SRLabs](https://srlabs.de/), [Trail of Bits](https://www.trailofbits.com/) and [Slow Mist](https://www.slowmist.com/en/).

![Image for post](https://miro.medium.com/max/1730/1*hKvzkJVXDmSA9OU7NhFLuA.jpeg)

The scope of the audit included all runtime implementations of Acala including ecosystem module RenVM, the community maintained ORML modules that Acala depends on, as well as the front-end interface for Acala’s DApp. So far SRLabs and Slow Mist have completed their audits, and the Trail of Bits audit is scheduled to commence in Jan 2021.

# The Report & Fixes

The SRLabs audit found 0 Critical, 1 High, 7 Medium and 2 Low-level issues.

The SlowMist audit found 0 Critical, 0 High, 1 Medium and 1 Low-level issue.

The one high-level issue regarding weight assignment was a planned task yet to be implemented at the time of the audit. We have now completed benchmarking and finalized appropriate weights for all [extrinsic](https://substrate.dev/docs/en/knowledgebase/learn-substrate/extrinsics) (aka signed/unsigned transactions, and inherits — info included in a block but not gossiped).

All other network security related issues have been addressed and reviewed by the auditors. There are two application-related issues (#5 and #8 in SRLabs report) are general DeFi issues such as DeX front-running, which yet to have a satisfactory solution. We are addressing it from a risk management perspective by setting safe parameters. Beyond that, we are seeking further economic audits that use simulation-based market stress testing so that we can evaluate vulnerabilities and market risks at a scaled volume and value.

The full report from SRLabs and SlowMist are [here](https://github.com/AcalaNetwork/Acala/tree/master/audit)

# Moving Forward

Audits are only one part of our effort in ensuring security and managing risks. All of Acala’s runtime codebases are audited, and upon genesis, all balances and governance decisions will be publicly verifiable. Our [Bug Bounty Program](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#runtime-bug-bounty) is also an important part to keep our codebase secure, and we encourage developers to dig into our code and report vulnerabilities. We believe transparency, time, and value are the true tests for the security of a network and protocols; so please be vigilant and help us make Acala safer and more secure for everyone.

# Join Us

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launch, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot, making fast and easy to use financial applications available to everyone. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.
