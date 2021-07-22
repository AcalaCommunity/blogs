# การสร้าง Acala — พฤศจิกายน & ธันวาคม 2020

## บทสรุปของการประมูล Crowdloan และ Parachain ของ Karura, EVM, Ampleforth, Open Oracle Gateway สำหรับ Polkadot และอื่นๆ

![Image for post](https://miro.medium.com/max/1600/0*FFQACU02-W0imy_8)

สุขสันต์วันหยุด!  นี่เป็นรุ่นพิเศษของ Building Acala ที่จะนำเสนอการอัปเดตสำหรับเดือนพฤศจิกายนและธันวาคม 2020 หากคุณยังใหม่กับ Acala ยินดีต้อนรับ! [Acala](http://acala.network/) เป็นศูนย์กลางทางการเงินแบบกระจายอำนาจของ Polkadot ที่ทำให้ใช้งานหรือสร้างแอปพลิเคชันทางการเงินได้อย่างรวดเร็วและง่ายดาย เพิ่มประสิทธิภาพการเทรดและประหยัดเวลา

สองสามเดือนที่ผ่านมาเป็นเรื่องเกี่ยวกับการสร้างและการตอบแทน — เราได้ทำการพัฒนาครั้งสำคัญใน EVM และความสามารถในการปรับแต่งและความเข้ากันได้ของ Substrate, ปรับใช้ Open Oracle Gateway โดยมี Acala, Band และ DIA เป็นผู้ให้บริการเครือข่าย oracle เริ่มต้น ยินดีกับ Ampleforth ในการเข้าร่วมระบบนิเวศและนำ AMPL ถึง Acala/Polkadot และเปิดตัวแคมเปญ Crowdloan ของ Karura (DeFi Hub ของ Kusama) ก่อนการประมูลและการเปิดตัว Parachain ที่จะเกิดขึ้น

# อัพเดทการวิจัย & การพัฒนา

- **Project Bodhi** เป็นสแต็ค EVM ที่ประกอบและสร้างสรรค์ได้บน Substrate เพื่อมอบความสามารถในการปรับแต่งแบบฟูลสแตกระหว่าง EVM และรันไทม์สำหรับนักพัฒนา และประสบการณ์การใช้งานแบบ cross-chain ในกระเป๋าเงินเดียวสำหรับผู้ใช้ อ่านต่อ [บน Github](https://github.com/w3f/Open-Grants-Program/blob/master/applications/project_bodhi.md). รายละเอียดเพิ่มเติมจะถูกเปิดเผยในโพสต์และการเดโม่ที่กำลังจะมาถึง
- **Open Oracle Gateway** คือแนวทางของเราในการสร้างเฟรมเวิร์กออราเคิลที่เปิดกว้าง ครอบคลุม และกระจายอำนาจมากขึ้นสำหรับฮับ Acala DeFi, Polkadot, ระบบนิเวศ Kusama และอื่นๆ Gateway ช่วยให้เครือข่าย oracles หลายแห่งสามารถให้บริการกับ DApps ใด ๆ ที่ปรับใช้หรือเชื่อมต่อกับ Acala ในขณะที่เพลิดเพลินกับคุณภาพของบริการและค่าธรรมเนียมการทำธุรกรรมฟรี เกตเวย์เปิดใช้งานและทำงานบน Acala testnet, Acala, Band และ DIA ซึ่งเป็นผู้ให้บริการเครือข่ายออราเคิลเริ่มต้น อ่านต่อด้านล่าง:

  [ขอแนะนำ Open Oracle Gateway สำหรับ Polkadot](https://medium.com/acalanetwork/introducing-the-open-oracle-gateway-for-polkadot-3554f7a4254e)

  ![Image for post](https://miro.medium.com/max/3200/0*vgXF6h9S3o0-qMgL)

- **Ampleforth บน Acala/Polkadot**: AMPL สกุลเงินที่ปรับฐานและโครงสร้างทางการเงินที่ยืดหยุ่นจะมีอยู่ใน Polkadot ผ่านเครือข่าย Acala Ample จะกลายเป็นโทเค็นค่าธรรมเนียมระดับ 1 บน Acala สัญญา Ampleforth จะถูกนำไปใช้กับ EVM ของ Acala โดยมีการเปลี่ยนแปลงเพียงเล็กน้อยในขณะที่เพลิดเพลินกับการผสานรวมกับ DeFi ดั้งเดิมและสภาพคล่องของ Acala อย่างราบรื่นด้วย Project Bodhi อ่านต่อด้านล่าง:

  [Ampleforth ซึ่งเป็น Building Block ของ DeFi นำการรีเบสสกุลเงินและการเงินที่ยืดหยุ่นมาสู่ Acala และ...](https://medium.com/acalanetwork/ampleforth-a-defi-building-block-brings-rebasing-currency-and-elastic-finance-to-acala-and-fd1388e8e8fc)

- **Decentralized Sovereign Wealth Fund:** คือ DAO รุ่นต่อไปและ AUM ที่ไม่สามารถ fork ได้ อ่านเพิ่มเติมใน [บล็อก](https://www.parity.io/defi-on-polkadot-an-ecosystem-overview/#:~:text=Polkadot%20%2D%20a%20network%20protocol%20that,to%20be%20transferred%20across%20blockchains.) ของ Parity

  [กองทุนความมั่งคั่งอธิปไตยแบบกระจายอำนาจของ Acala — DAO รุ่นต่อไป & AUM ที่ไม่สามารถ fork ได้](https://medium.com/acalanetwork/acalas-decentralized-sovereign-wealth-fund-a-next-gen-dao-unforkable-aum-80f8c23d8f27)

- **Security Audit:** SRLabs and Slow Mist have completed their audits on Acala including all runtime implementations, ecosystem module RenVM, the community maintained ORML modules that Acala depends on, as well as the front-end interface for Acala’s DApp. The Trail of Bits audit is scheduled to commence in Jan 2021. Read more below:

  [Acala Security Audit](https://medium.com/acalanetwork/acala-security-audit-edd1850e27aa)

# Launch Plan & Community

- **Launch Timeline:** Rococo parachain testnet V1 has been released and will accept parachains early Jan 2021. This is a solid technical indicator of parachain readiness. If testing and auditing all go as planned, then Kusama will enable parachain auctions, followed by Polkadot. Acala will be amongst the first parachains and launch on both networks.

  ![Image for post](https://miro.medium.com/max/2376/1*a-5oImcqeMrXczG4RZK7-Q.png)

- **Karura’s Parachain Launch Crowdloan Waitlist is Open:** Karura (Acala’s sister network on Kusama) will host the first crowdsourced parachain launch. The **Crowdloan** model is pioneering a new way of fair network bootstrapping: KSM holders lock their tokens to help us lease a parachain slot and gain access to Kusama’s shared security, they will get all principles back at the end of the lease, while receiving KAR tokens as reward for their support. The goal is to distribute our tokens to as many KSM holders as possible, and a bonus referral program is set up to achieve this goal. The campaign started a few days ago, and now already attracted **_3.3k people joining the Crowdloan waitlist!_ Join Karura’s Crowdloan waitlist** [**here**](https://twitter.com/AcalaNetwork/status/1339431441139154945?s=20) and view the Karura Crowdloan [website](https://acala.network/kar-crowdloan).

- **The Substrate Runtime Developer Academy** launched by Acala, Industry Connect and Parity, and supported by wide range of community partners is a professional level program to help developers building production-grade applications for Polkadot. The first intake has 52 students from 19 countries inc Argentina, Brazil, Russia, US, Turkey and more. Polkadot Treasury has recently granted the program a scholarship fund of 643 DOTs to support students in need. **Read more** [**on the Treasury proposal**](https://polkadot.polkassembly.io/treasury/28) **or** [**sign up for the next cohort (Feb 2021) now**](https://www.industryconnect.org/substrate-runtime-developer-academy/)**!**

- **Vote Acala for Polkadot & Kusama Council Member:** for a more enlightened DeFi future. During our tenure, we have participated in 37 Kusama council votes and 37 Polkadot council votes.

- **Token Distribution:** one of our goals is to distribute our tokens as widely and fairly as possible. Looking back 2020, we have distributed roughly 1 hundred thousand ACA and 3.5 million KAR tokens to the community through testnet participation — the Mandala Festivals, bounty programs and hackathon prizes.

# Events & Media

- **Polkadot Decoded:** the first Polkadot conference has attracted over 6,000 attendants, watch Acala’s co-founder Ruitao Su’s presentation [here](https://twitter.com/AcalaNetwork/status/1334596628951355392?s=20).
- **Hackathons:** we have supported the following hackathons:
- Polkadot’s Hello World [on Gitcoin](https://gitcoin.co/hackathon/polkadot/?)
- Polkadot Encode Hackathon [here](https://medium.com/encode-club/encode-hack-club-announcing-polkadot-c7cc6cc12920)
- Substrate Dorahacks in Hangzhou [here](https://twitter.com/DoraHacks/status/1339926282797105152?s=20)
- Acala’s co-founder Ruitao on Pantera’s Conference Calls “Deconstructing DeFi” with Alchemy’s co-founder Joe Lau [here](https://twitter.com/PanteraCapital/status/1323258191841558531?s=20)
- [DeFi Startup Acala to Build New Oracle Network For Polkadot Ecosystem](https://coinmarketcap.com/zh/headlines/news/defi-startup-acala-to-build-new-oracle-network-for-polkadot-ecosystem/) by CoinMarketCap
- [DeFi on Polkadot](https://cointelegraph.com/news/defi-on-polkadot-an-alt-chain-with-interoperability-on-the-horizon) by Cointelegraph

<img alt="Image for post" class="t u v hu aj" src="https://miro.medium.com/max/2136/0\*-urwFFbwsGGsBSk8" width="1068" height="1600" srcSet="https://miro.medium.com/max/552/0\*-urwFFbwsGGsBSk8 276w, https://miro.medium.com/max/1104/0\*-urwFFbwsGGsBSk8 552w, https://miro.medium.com/max/1280/0\*-urwFFbwsGGsBSk8 640w, https://miro.medium.com/max/1400/0\*-urwFFbwsGGsBSk8 700w" sizes="700px" />

# Join Us

[Discord](https://discord.gg/vdbFVCH) | [Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launches on Polkadot and Kusama, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

[Work with us](https://jobs.lever.co/acala/) — we’re hiring 😎

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot that makes it fast and easy to use or build financial applications, improving trading efficiency and saving valuable time. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de-facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.

# About Karura

[Karura](http://acala.network/karura-crowdloan) is the decentralized financial hub of Kusama. The network is built as Acala’s sister network with nearly the same codebase — the two platforms enable a scalable, user-friendly, and fast cross-chain DeFi ecosystem for Kusama and Polkadot. Karura’s parachain is a fast-moving and powerful platform that enables efficient, inexpensive, and sophisticated financial applications, improving trading effectiveness and saving time. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Kusama and Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations.
