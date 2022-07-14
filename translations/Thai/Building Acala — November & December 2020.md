# การสร้าง Acala — พฤศจิกายน & ธันวาคม 2020

## บทสรุปของการประมูล Crowdloan และ Parachain ของ Karura, EVM, Ampleforth, Open Oracle Gateway สำหรับ Polkadot และอื่นๆ

![รูปสำหรับโพสต์](https://miro.medium.com/max/1600/0*FFQACU02-W0imy_8)

สุขสันต์วันหยุด!  นี่เป็นรุ่นพิเศษของ Building Acala ที่จะนำเสนอการอัปเดตสำหรับเดือนพฤศจิกายนและธันวาคม 2020 หากคุณยังใหม่กับ Acala ยินดีต้อนรับ! [Acala](http://acala.network/) เป็นศูนย์กลางทางการเงินแบบกระจายอำนาจของ Polkadot ที่ทำให้ใช้งานหรือสร้างแอปพลิเคชันทางการเงินได้อย่างรวดเร็วและง่ายดาย เพิ่มประสิทธิภาพการเทรดและประหยัดเวลา

สองสามเดือนที่ผ่านมาเป็นเรื่องเกี่ยวกับการสร้างและการตอบแทน — เราได้ทำการพัฒนาครั้งสำคัญใน EVM และความสามารถในการปรับแต่งและความเข้ากันได้ของ Substrate, ปรับใช้ Open Oracle Gateway โดยมี Acala, Band และ DIA เป็นผู้ให้บริการเครือข่าย oracle เริ่มต้น ยินดีกับ Ampleforth ในการเข้าร่วมระบบนิเวศและนำ AMPL ถึง Acala/Polkadot และเปิดตัวแคมเปญ Crowdloan ของ Karura (DeFi Hub ของ Kusama) ก่อนการประมูลและการเปิดตัว Parachain ที่จะเกิดขึ้น

# อัพเดทการวิจัย & การพัฒนา

- **Project Bodhi** เป็นสแต็ค EVM ที่ประกอบและสร้างสรรค์ได้บน Substrate เพื่อมอบความสามารถในการปรับแต่งแบบฟูลสแตกระหว่าง EVM และรันไทม์สำหรับนักพัฒนา และประสบการณ์การใช้งานแบบ cross-chain ในกระเป๋าเงินเดียวสำหรับผู้ใช้ อ่านต่อ [บน Github](https://github.com/w3f/Open-Grants-Program/blob/master/applications/project_bodhi.md). รายละเอียดเพิ่มเติมจะถูกเปิดเผยในโพสต์และการเดโม่ที่กำลังจะมาถึง
- **Open Oracle Gateway** คือแนวทางของเราในการสร้างเฟรมเวิร์กออราเคิลที่เปิดกว้าง ครอบคลุม และกระจายอำนาจมากขึ้นสำหรับฮับ Acala DeFi, Polkadot, ระบบนิเวศ Kusama และอื่นๆ Gateway ช่วยให้เครือข่าย oracles หลายแห่งสามารถให้บริการกับ DApps ใด ๆ ที่ปรับใช้หรือเชื่อมต่อกับ Acala ในขณะที่เพลิดเพลินกับคุณภาพของบริการและค่าธรรมเนียมการทำธุรกรรมฟรี เกตเวย์เปิดใช้งานและทำงานบน Acala testnet, Acala, Band และ DIA ซึ่งเป็นผู้ให้บริการเครือข่ายออราเคิลเริ่มต้น อ่านต่อด้านล่าง:

  [ขอแนะนำ Open Oracle Gateway สำหรับ Polkadot](https://medium.com/acalanetwork/introducing-the-open-oracle-gateway-for-polkadot-3554f7a4254e)

  ![รูปสำหรับโพสต์](https://miro.medium.com/max/3200/0*vgXF6h9S3o0-qMgL)

- **Ampleforth บน Acala/Polkadot**: AMPL สกุลเงินที่ปรับฐานและโครงสร้างทางการเงินที่ยืดหยุ่นจะมีอยู่ใน Polkadot ผ่านเครือข่าย Acala Ample จะกลายเป็นโทเค็นค่าธรรมเนียมระดับ 1 บน Acala สัญญา Ampleforth จะถูกนำไปใช้กับ EVM ของ Acala โดยมีการเปลี่ยนแปลงเพียงเล็กน้อยในขณะที่เพลิดเพลินกับการผสานรวมกับ DeFi ดั้งเดิมและสภาพคล่องของ Acala อย่างราบรื่นด้วย Project Bodhi อ่านต่อด้านล่าง:

  [Ampleforth ซึ่งเป็น Building Block ของ DeFi นำการรีเบสสกุลเงินและการเงินที่ยืดหยุ่นมาสู่ Acala และ...](https://medium.com/acalanetwork/ampleforth-a-defi-building-block-brings-rebasing-currency-and-elastic-finance-to-acala-and-fd1388e8e8fc)

- **Decentralized Sovereign Wealth Fund:** คือ DAO รุ่นต่อไปและ AUM ที่ไม่สามารถ fork ได้ อ่านเพิ่มเติมใน [บล็อก](https://www.parity.io/defi-on-polkadot-an-ecosystem-overview/#:~:text=Polkadot%20%2D%20a%20network%20protocol%20that,to%20be%20transferred%20across%20blockchains.) ของ Parity

  [กองทุนความมั่งคั่งอธิปไตยแบบกระจายอำนาจของ Acala — DAO รุ่นต่อไป & AUM ที่ไม่สามารถ fork ได้](https://medium.com/acalanetwork/acalas-decentralized-sovereign-wealth-fund-a-next-gen-dao-unforkable-aum-80f8c23d8f27)

- **Security Audit:** SRLabs และ Slow Mist ได้เสร็จสิ้นการตรวจสอบบน Acala รวมถึงการใช้งานรันไทม์ทั้งหมด โมดูลระบบนิเวศ RenVM ชุมชนดูแลโมดูล ORML ที่ Acala พึ่งพา ตลอดจนอินเทอร์เฟซ front-end สำหรับ DApp ของ Acala . การตรวจสอบ Trail of Bits มีกำหนดจะเริ่มในเดือนมกราคม 2021 อ่านต่อด้านล่าง:

  [Acala Security Audit](https://medium.com/acalanetwork/acala-security-audit-edd1850e27aa)

# เปิดตัวแผน & Community

- **ไทม์ไลน์การเปิดตัว:** Rococo parachain testnet V1 ได้รับการเผยแพร่แล้ว และจะยอมรับ parachain ในต้นเดือนมกราคม 2021 นี่เป็นตัวบ่งชี้ทางเทคนิคที่ชัดเจนของความพร้อมของ Parachain หากการทดสอบและการตรวจสอบเป็นไปตามแผนที่วางไว้ Kusama จะเปิดใช้งานการประมูลแบบ Parachain ตามด้วย Polkadot Acala จะเป็นหนึ่งใน Parachains ตัวแรกและเปิดตัวบนทั้งสองเครือข่าย

  ![รูปสำหรับโพสต์](https://miro.medium.com/max/2376/1*a-5oImcqeMrXczG4RZK7-Q.png)

- **Parachain ของ Karura เปิดตัว Crowdloan Waitlist ที่เปิดอยู่:** Karura (เครือข่ายน้องสาวของ Acala บน Kusama) จะจัดงานเปิดตัว Parachain แบบคราวด์ซอร์ซเป็นครั้งแรก โมเดล **Crowdloan** กำลังบุกเบิกวิธีการใหม่ในการบูตเครือข่ายอย่างยุติธรรม: ผู้ถือ KSM ล็อคโทเค็นของตนเพื่อช่วยให้เราเช่าสล็อต parachain และเข้าถึงการรักษาความปลอดภัยที่ใช้ร่วมกันของ Kusama พวกเขาจะได้รับทั้งหมดกลับคืนมาเมื่อสิ้นสุดตามหลักการ ขณะที่รับโทเค็น KAR เป็นรางวัลสำหรับการสนับสนุน เป้าหมายคือการแจกจ่ายโทเค็นของเราให้กับผู้ถือ KSM ให้ได้มากที่สุด และมีการตั้ง referal program โบนัสเพื่อให้บรรลุเป้าหมายนี้ แคมเปญเริ่มต้นเมื่อไม่กี่วันก่อน และตอนนี้ดึงดูดผู้คน **_3.3k คนให้เข้าร่วมในรายการรอ Crowdloan!_ เข้าร่วมในรายชื่อรอ Crowdloan ของ Karura** [**ที่นี่**](https://twitter.com/AcalaNetwork/status/1339431441139154945?s=20) และดู Karura Crowdloan [เว็บไซต์](https://acala.network/kar-crowdloan).

- ** Substrate Runtime Developer Academy** ที่เปิดตัวโดย Acala, Industry Connect และ Parity และได้รับการสนับสนุนจากพันธมิตรในชุมชนที่หลากหลาย เป็นโปรแกรมระดับมืออาชีพที่จะช่วยนักพัฒนาสร้างแอปพลิเคชันระดับโปรดักชั่นสำหรับ Polkadot การรับเข้าเรียนครั้งแรกมีนักเรียน 52 คนจาก 19 ประเทศ รวมทั้งอาร์เจนตินา บราซิล รัสเซีย สหรัฐอเมริกา ตุรกี และอื่นๆ Polkadot Treasury ได้มอบทุนทุนการศึกษาจำนวน 643 DOTs ให้กับโครงการเพื่อสนับสนุนนักเรียนที่ต้องการความช่วยเหลือ **อ่านเพิ่มเติม** [**เกี่ยวกับข้อเสนอ Treasury**](https://polkadot.polkassembly.io/treasury/28) **หรือ** [**ลงชื่อสมัครใช้ในกลุ่มถัดไป (ก.พ. 2021) ตอนนี้**](https://www.industryconnect.org/substrate-runtime-developer-academy/)**! **

- **โหวต Acala สำหรับสมาชิกสภา Polkadot &  Kusama:** เพื่ออนาคต DeFi ที่กระจ่างแจ้งยิ่งขึ้น ในระหว่างดำรงตำแหน่ง เราได้เข้าร่วมในการโหวตของสภา Kusama 37 เสียง และคะแนนโหวตของสภา Polkadot 37 เสียง

- **การแจกจ่ายโทเค็น:** หนึ่งในเป้าหมายของเราคือแจกจ่ายโทเค็นของเราให้กว้างขวางและยุติธรรมที่สุด เมื่อมองย้อนกลับไปในปี 2020 เราได้แจกจ่าย ACA ประมาณ 1 แสนรายการและโทเค็น KAR 3.5 ล้านโทเค็นให้กับชุมชนผ่านการเข้าร่วม testnet — เทศกาล Mandala, โปรแกรมเงินรางวัล และรางวัลแฮกกาธอน

# กิจกรรม & สื่อ

- **Polkadot Decoded:** การประชุม Polkadot ครั้งแรกดึงดูดผู้เข้าร่วมกว่า 6,000 คน ชมการนำเสนอของ Ruitao Su ผู้ร่วมก่อตั้งของ Acala [ที่นี่](https://twitter.com/AcalaNetwork/status/1334596628951355392?s=20)
- **Hackathons:** เราได้สนับสนุน Hackathons ดังต่อไปนี้:
- Polkadot’s Hello World [บน Gitcoin](https://gitcoin.co/hackathon/polkadot/?)
- Polkadot Encode Hackathon [ที่นี่](https://medium.com/encode-club/encode-hack-club-announcing-polkadot-c7cc6cc12920)
- Substrate Dorahacks ใน Hangzhou [ที่นี่](https://twitter.com/DoraHacks/status/1339926282797105152?s=20)
- Ruitao ผู้ร่วมก่อตั้งของ Acala ในการประชุมของ Pantera “Deconstructing DeFi” กับ Joe Lau ผู้ร่วมก่อตั้งของ Alchemy [ที่นี่](https://twitter.com/PanteraCapital/status/1323258191841558531?s=20)
- [DeFi Startup Acala เพื่อสร้างเครือข่าย Oracle ใหม่สำหรับระบบนิเวศ Polkadot](https://coinmarketcap.com/zh/headlines/news/defi-startup-acala-to-build-new-oracle-network-for-polkadot-ecosystem/) โดย CoinMarketCap
- [DeFi บน Polkadot](https://cointelegraph.com/news/defi-on-polkadot-an-alt-chain-with-interoperability-on-the-horizon) โดย Cointelegraph

<img alt="รูปสำหรับโพสต์" class="t u v hu aj" src="https://miro.medium.com/max/2136/0\*-urwFFbwsGGsBSk8" width="1068" height="1600" srcSet="https://miro.medium.com/max/552/0\*-urwFFbwsGGsBSk8 276w, https://miro.medium.com/max/1104/0\*-urwFFbwsGGsBSk8 552w, https://miro.medium.com/max/1280/0\*-urwFFbwsGGsBSk8 640w, https://miro.medium.com/max/1400/0\*-urwFFbwsGGsBSk8 700w" sizes="700px" />

# ร่วมกับเรา

[Discord](https://discord.gg/vdbFVCH) | [Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

หากต้องการติดตามความคืบหน้าเกี่ยวกับการเปิดตัว Acala Parachain บน Polkadot และ Kusama โปรดสมัครรับข้อมูล [จดหมายข่าวของ Acala](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc)

[ทำงานกับเรา](https://jobs.lever.co/acala/) — เรากำลังหาผู้สนใจ 😎

# เกี่ยวกับ Acala

[Acala](http://acala.network/) เป็นศูนย์กลางทางการเงินแบบกระจายอำนาจของ Polkadot ที่ทำให้ใช้งานหรือสร้างแอปพลิเคชันทางการเงินได้อย่างรวดเร็วและง่ายดาย เพิ่มประสิทธิภาพการเทรดและประหยัดเวลา แพลตฟอร์มนำเสนอชุดพื้นฐานทางการเงิน: stablecoin ค้ำประกันที่มีความหลากหลายซึ่งได้รับการสนับสนุนจากทรัพย์สิน cross-chain เช่น Bitcoin อนุพันธ์ trustless staking และการแลกเปลี่ยนแบบกระจายอำนาจเพื่อปลดปล่อยสภาพคล่องและนวัตกรรมทางการเงินที่มีอำนาจ Acala เป็นแพลตฟอร์มเปิดตามความจริง(de facto) สำหรับแอปพลิเคชันด้านการเงินเพื่อใช้ smart contract หรือโปรโตคอลในตัวที่มีความสามารถ cross-chain, ความปลอดภัย และการเพิ่มประสิทธิภาพทางการเงิน

# เกี่ยวกับ Karura

[Karura](http://acala.network/karura-crowdloan) เป็นศูนย์กลางทางการเงินแบบกระจายอำนาจของ Kusama เครือข่ายนี้สร้างขึ้นในฐานะเครือข่ายน้องสาวของ Acala ที่มีพื้นฐานโค้ดเกือบเหมือนกัน — ทั้งสองแพลตฟอร์มช่วยให้ระบบนิเวศ DeFi cross-chain ปรับขนาดได้ ใช้งานง่าย และรวดเร็วสำหรับ Kusama และ Polkadot Parachain ของ Karura เป็นแพลตฟอร์มที่เคลื่อนไหวรวดเร็วและทรงพลังที่ช่วยให้แอปพลิเคชันทางการเงินมีประสิทธิภาพ ราคาไม่แพง และซับซ้อน, ปรับปรุงประสิทธิภาพการซื้อขายและประหยัดเวลา แพลตฟอร์มดังกล่าวนำเสนอชุดของพื้นฐานทางการเงิน: เหรียญ stablecoin แบบหลายหลักประกันที่ได้รับการสนับสนุนจากสินทรัพย์ cross-chain เช่น Kusama และ Bitcoin อนุพันธ์การ Stake แบบ trustless และการแลกเปลี่ยนแบบกระจายอำนาจเพื่อปลดปล่อยสภาพคล่องและนวัตกรรมทางการเงินด้านอำนาจ
