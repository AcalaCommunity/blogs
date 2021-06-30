# Acala Security Audit

![Image for post](https://miro.medium.com/max/8000/1*yhydywHe1k2421hd6xqhFQ.jpeg)

ที่ acala เราเชื่อว่า ผู้ใช้แต่ละคน ไม่ใช่องค์กร ควรเป็นคนบริหารเงินของตัวเอง ภารกิจของเราคือการสนับสนุนและดูแล แอปพลิเคชั่นทางการเงินของ Web 3.0 -- เว็บที่มีการกระจายอำนาจอย่างแท้จริง และ "trustless" (ไม่จำเป็นต้องเชื่อถือ) อนาคตทางการเงินที่แฟร์และเปิดกว้างมากขึ้นคือสิ่งที่เราหวังที่จะเปิดผ่านแพลตฟอร์ม smart contract และ โปรโตคอลของเรา -- Stablecoin แบบกระจายอำนาจ, การ staking สภาพคล่อง และ การแลกเปลี่ยนแบบกระจายอำนาจ

นั่นหมายถึง ระบบรักษาความปลอดภัยของ blockchain และ โปรโตคอลของ Acala คือสิ่งที่เราให้ความสำคัญสูงสุด เราได้ทุ่มเทความพยายามอย่างมากในการพัฒนาแพลตฟอร์มและโปรโตคอลที่เกี่ยวข้องซึ่งเราเชื่อว่าปลอดภัยและเชื่อถือได้ เรายังได้ทุ่มเทสิ่งที่ดีที่สุดในธุรกิจเพื่อช่วยตรวจสอบ โค้ดของเรา ซึ่งได้แก่ [SRLabs](https://srlabs.de/), [Trail of Bits](https://www.trailofbits.com/) และ [Slow Mist](https://www.slowmist.com/en/)

![Image for post](https://miro.medium.com/max/1730/1*hKvzkJVXDmSA9OU7NhFLuA.jpeg)

ขอบเขตของการ audit รวมถึงการใช้งานรันไทม์ทั้งหมดของ Acala รวมทั้งโมดูล ecosystem ของ RenVM, community ที่ดูแลโมดูล ORML ที่ Acala พึ่งพาตลอดจนถึงอินเทอร์เฟซ front-end สำหรับ DApp ของ Acala ซึ่งปัจจุบัน SRLabs และ Slow Mist ได้ audit เรียบร้อยแล้ว และการตรวจสอบ Trail of Bits มีกำหนดจะเริ่มในเดือนมกราคม 2021

# The Report & Fixes

การตรวจสอบ SRLabs พบปัญหาที่สำคัญ 0 รายการ, สูง 1 รายการ, ปานกลาง 7 รายการ และระดับต่ำ 2 รายการ

การตรวจสอบ SlowMist พบปัญหาที่สำคัญ 0 รายการ, สูง 0 รายการ, ปานกลาง 1 รายการ และระดับต่ำ 1 รายการ

โดยปัญหาระดับสูงรายการหนึ่งนั้นเกี่ยวกับการกำหนดน้ำหนักที่มอบหมายที่ได้วางแผนไว้นั้นยังไม่ได้ดำเนินการ ในขณะที่ทำการตรวจสอบ ตอนนี้เราได้ทำการเปรียบเทียบและสรุปการให้น้ำหนักที่เหมาะสมสำหรับ [extrinsic](https://substrate.dev/docs/en/knowledgebase/learn-substrate/extrinsics) ทั้งหมดแล้ว (ธุรกรรมที่ลงชื่อ/ไม่ได้ลงชื่อ และการรับช่วงต่อ — ข้อมูลถูกรวมอยู่ในบล็อกแต่ไม่ถูกพบ)

ปัญหาด้านความปลอดภัยของ network อื่นๆ ทั้งหมดได้รับการแก้ไขและตรวจสอบโดยผู้ตรวจสอบแล้ว There are two application-related issues (#5 and #8 in SRLabs report) are general DeFi issues such as DeX front-running, which yet to have a satisfactory solution. We are addressing it from a risk management perspective by setting safe parameters. Beyond that, we are seeking further economic audits that use simulation-based market stress testing so that we can evaluate vulnerabilities and market risks at a scaled volume and value.

The full report from SRLabs and SlowMist are [here](https://github.com/AcalaNetwork/Acala/tree/master/audit)

# Moving Forward

Audits are only one part of our effort in ensuring security and managing risks. All of Acala’s runtime codebases are audited, and upon genesis, all balances and governance decisions will be publicly verifiable. Our [Bug Bounty Program](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#runtime-bug-bounty) is also an important part to keep our codebase secure, and we encourage developers to dig into our code and report vulnerabilities. We believe transparency, time, and value are the true tests for the security of a network and protocols; so please be vigilant and help us make Acala safer and more secure for everyone.

# Join Us

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launch, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot, making fast and easy to use financial applications available to everyone. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.
