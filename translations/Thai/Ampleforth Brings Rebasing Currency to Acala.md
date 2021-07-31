# Ampleforth ซึ่งเป็น Building Block ของ DeFi นำการรีเบสสกุลเงินและการเงินที่ยืดหยุ่นมาสู่ Acala และ Polkadot

## Ampleforth จะเปิดตัวใน Acala (Polkadot) ในต้นปีหน้า

![Image for post](https://miro.medium.com/max/1600/0*u9U9isEmIWMS9LJl)

# อิสระเสรี เงินแบบ multichain

AMPL โดยทีมงาน [Ampleforth](https://www.ampleforth.org/) เป็นสกุลเงินดิจิทัลที่เป็นอิสระอย่างแท้จริงซึ่งนำเงินแบบ chain-agnostic, non-dilutive มาสู่การเงินแบบกระจายอำนาจ จะมีให้บริการในเครือข่าย Acala เร็วๆนี้

Ampleforth ได้แนะนำโลกให้รู้จักกับ rebase ซึ่งเป็นกลไกเฉพาะที่ช่วยให้มั่นใจถึงความสมดุลของราคาและซัพพลาย Ampleforth นั้นเหมือนกับ Bitcoin เว้นแต่ว่าสามารถใช้เพื่อกำหนดสัญญาที่เสถียรได้ เช่นเดียวกับ Bitcoin AMPL ไม่มีหลักประกัน แต่ที่ไม่เหมือน Bitcoin, AMPL มีนโยบายของซัพพลายที่ยืดหยุ่น สกุลเงิน Ampleforth จะ 'ปรับฐาน' ซัพพลายโดยอัตโนมัติตามสัดส่วนและ non-dilutive เพื่อตอบสนองต่อความผันผวนของราคา แนวทางนี้เป็นกุญแจสำคัญในการทำให้สัญญามีเสถียรภาพ ซึ่งเป็นการป้องกันความเสี่ยงที่สำคัญต่อความผันผวนของราคาที่เกี่ยวข้องกับ smart contract ในปัจจุบัน ความสามารถนี้ทำให้ AMPL เป็นส่วนประกอบสำคัญสำหรับระบบนิเวศ DeFi

[Ampleforth Everywhere](https://medium.com/ampleforth/independent-currency-in-a-multi-chain-world-67032dce8296) เป็นวิสัยทัศน์ระยะยาวของทีม Ampleforth ในการนำ AMPL มาสู่บล็อกเชนหลายแห่ง และดำเนินนโยบายการเงินเพื่อควบคุมซัพพลายให้สอดคล้องกับความต้องการของตลาด

[Ampleforth มีแนวโน้มที่จะเปิดตัวใน Acala (Polkadot)](https://www.ampltalk.org/app/forum/announcements-22/topic/multichain-ampleforth-231/?utm_source=AMPLTwtr_Announce_multichain_3chains_12_2_20&utm_medium=AMPLTwtr_Announce_multichain_3chains_12_2_20&utm_campaign=AMPLTwtr_Announce_multichain_3chains_12_2_20) ในต้นปีหน้า ทำให้เป็นเงินอิสระแบบ multichain แรกที่ให้บริการชุมชน crypto และ DeFi แบบ cross-chain ในวงกว้าง

Polkadot เปิดใช้งานเครือข่ายของบล็อกเชนที่เชื่อมต่อถึงกัน นำเสนอการสื่อสารระหว่างเชนและความปลอดภัยที่ใช้ร่วมกันเพื่อเชื่อมโยงเชนที่มีอยู่ เช่น Ethereum และ Bitcoin กับ Parachain จำนวนมากที่เชื่อมต่ออยู่ Polkadot มีสถาปัตยกรรมแบบ hub-and-spoke โดยที่เครือข่ายที่ทำงานในปัจจุบันคือฮับหรือที่เรียกว่า Relay Chain ที่ให้การรักษาความปลอดภัยเครือข่าย Proof-of-Stake และจะเป็นจุดยึดสำหรับการสื่อสาร cross-chain อย่างไรก็ตาม มันไม่มีการใช้งานระดับแอปพลิเคชันใดๆ หรือความสามารถของ smart contract ที่จะรับรู้โดยแต่ละ parachains และ parathreads

Acala is one of the leading parachains in the Polkadot ecosystem that is optimized for DeFi, often serves as a landing pad and DeFi hub of Polkadot. DApps deploying on Acala not only gain immediate access to Polkadot’s multi-chain ecosystem via cross-chain message passing mechanism ([XCMP](https://wiki.polkadot.network/docs/en/learn-crosschain)), but also have full access to Acala’s existing DeFi primitives such as DeX, user base, and liquidity.

# AMPL on Acala (Polkadot)

We’re pleased to welcome Ampleforth to Acala’s Ecosystem Program, as well as the ever-growing Polkadot ecosystem.

Ampleforth Everywhere will have a single monetary policy that automatically adjusts supply based on demand (called ‘rebase’) on multiple blockchains. The user flow looks like this:

- Value-transfer: A user is able to transfer AMPLs from their wallet on one chain to another wallet on a different chain.
- State Transfer: The monetary policy is able to call rebase() on the token contract of a different chain, or otherwise sync its state to the other chain to adjust supply.

Specifically, Ampleforth’s deployment on Acala will bring these benefits to the users

1.  Enable Ample money on Polkadot via Acala network
2.  Ample will become a 1st-class fee token on Acala, meaning users can pay AMPLs as fees when transferring AMPLs
3.  Ampleforth contracts will be deployed on Acala’s EVM with minimal changes while enjoying seamless integration with Acala’s DeFi primitives e.g. list directly on Acala Swap DeX.
4.  Transfer AMPL between Ethereum and Acala/Polkadot: RenVM will initially provide an Ethereum to Acala (Polkadot) bridge that will be used for value transfer and state transfer. Meanwhile, ChainBridge is considered as an alternative solution, while Snowfork’s trustless Ethereum bridge is also considered as a fully decentralized bridge option once it becomes available.

Technically Acala EVM is powered by [Project Bodhi](https://github.com/w3f/Open-Grants-Program/blob/master/applications/project_bodhi.md) — a composable and innovative EVM stack on [Substrate](https://www.substrate.io/) — a customizable blockchain framework used for building Polkadot, Kusama, Acala, and various types of blockchains. Project Bodhi has recently been awarded Web3 Foundation Open Grant to deliver full-stack composability between EVM and runtimes for developers, and a single-wallet cross-chain experience for users. More details will be revealed in an upcoming post.

# What’s Next

We are also collaborating with Ren to make RenVM Ethereum to Acala (Polkadot) bridge available in early 2021. Then Ampleforth contracts can be deployed on Acala mainnet, making AMPLs one of the first cross-chain assets available on Polkadot, and help realize the vision of Ampleforth Everywhere. Together with Polkadot and other ecosystem collaborators, Acala is poised to bring the cross-chain DeFi ecosystem and liquidity together, and empower more open finance innovations.

_Click here to_ [_learn more about Ampleforth_](https://www.ampleforth.org/quickstart/)_._

_Interested in a career in decentralized finance? If you enjoy working on high-impact, web3 and DeFi challenges, check out_ [_our open positions_](https://jobs.lever.co/acala/) _here. We’d love to hear from you._

**Join Acala**

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki)

To keep up to date with progress on the Acala parachain launch, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

# About Ampleforth

Ample is a new base-money cryptocurrency with elastic supply and rules-based governance. Ample naturally adapts to changes in demand by universally expanding or contracting supply, these changes affect all wallets equally, ensuring AMPL remains non-dilutive like Bitcoin. Ample supply expands or contracts by smart contract according to a rules-based monetary policy. Ample is not correlated with or derived from any other asset. Ample is a new base-money primitive for building the future of decentralized finance.

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot, making it fast and easy to use financial applications available to everyone. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de-facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.
