# Building Acala — ต.ค. 2020 | บทนำสู่ Karura — ศูนย์กลาง DeFi ของ Kusama, Parachain Lease Offer (PLO) & การบูรณาการ EVM

![Image for post](https://miro.medium.com/max/1600/0*hmK9ex3hJqibgvrl)

ถึงเวลาสำหรับ **Building Acala** เวอร์ชันเดือนตุลาคม 2020 และหากคุณเพิ่งเริ่มใช้ Acala เรายินดีต้อนรับ! [Acala](http://acala.network/) เป็นศูนย์กลางทางการเงินแบบกระจายอำนาจของ Polkadot ที่ทำให้ใช้งานหรือสร้างแอปพลิเคชันทางการเงินได้อย่างรวดเร็วและง่ายดาย เพิ่มประสิทธิภาพการเทรดและประหยัดเวลา

เมื่อเดือนที่แล้ว ทีมงานได้มุ่งสร้างการรวม EVM สนับสนุนทีมที่ใช้งานบน Acala และเปิดตัว Karura — DeFi Hub ของ Kusama ผ่าน Parachain Lease Offer (PLO) & Paradrop

# **อัพเดทการพัฒนา**

- **ความเข้ากันได้ของ Ethereum และ Smart Contracts**: เราได้พัฒนา EVM และ Smart Contracts ที่ทำงานร่วมกับ Acala ได้ดียิ่งขึ้น ความแตกต่างที่นี่คือสัญญา _ไม่มีอยู่ในแซนด์บ็อกซ์อีกต่อไป แต่สามารถเขียนด้วย DeFi primitive ของ Acala_ (stablecoin, DeX, staking Derivatives และอื่นๆ) _เคาะที่ฐานผู้ใช้ของ Acala สภาพคล่องและความสามารถ cross-chain_ และเปิดประตูสู่ตลาดที่ใหญ่ขึ้นมากในระบบนิเวศน์ Parachain ของ Polkadot รายละเอียดเพิ่มเติมจะประกาศเร็ว ๆ นี้

- **การตรวจสอบความปลอดภัย:** เราได้เสร็จสิ้นการตรวจสอบความปลอดภัยตามแผนแล้ว 2/3 ซึ่งรวมถึงการตรวจสอบจาก SRLabs และการตรวจสอบที่กำลังจะมีขึ้นจาก Trail of Bits รายละเอียดเพิ่มเติมเกี่ยวกับการตรวจนี้จะเปิดเผยในอีกไม่กี่สัปดาห์ข้างหน้า

- **การสนับสนุน NFT:** Acala ได้สร้าง [พาเลท NFT](https://github.com/open-web3-stack/open-runtime-module-library/tree/master/nft) ทั่วไป (หรือเรียกว่าโมดูล) เพื่อรองรับนวัตกรรม NFT บน Acala เช่น ผู้ให้บริการ Rarible หรือผู้ให้บริการ NFT รายอื่นๆ สามารถปรับใช้ smart contract เพื่อใช้ประโยชน์จากการสร้างบล็อก DeFi ของ Acala ได้อย่างง่ายดาย Kusama ได้นำโมดูลเดียวกันมาใช้เพื่อเปิดใช้งานการสนับสนุน NFT ดั้งเดิมบน Kusama Relay chain อ่านต่อ [ที่นี่](https://kusama.polkassembly.io/post/303#86924943-429c-4c05-a2fe-e7bef735b2a4).

# **เปิดตัวอัปเดต**

- **Acala จะเปิดตัวเครือข่าย Karura บน Kusama (**[**Medium**](https://medium.com/acalanetwork/introducing-karura-acalas-defi-parachain-on-kusama-af2f2695b07a)**)** — Karura เป็นเครือข่ายน้องสาวของ Acala และศูนย์กลาง DeFi สำหรับ Kusama กระบวนการเปิดตัวบน Kusama อาจใช้เวลาไม่ถึงเดือน สัญญาณที่ดีคือเมื่อฟังก์ชัน Parachain พร้อมบน testnet Rococo

- Karura จะเป็นเจ้าภาพจัดงาน **Parachain Lease Offering (PLO)** และ **Paradrop (**[**Medium**](https://medium.com/acalanetwork/karuras-approach-to-the-upcoming-parachain-lease-offering-plo-on-kusama-12fbf09ee463) **&**

**Tweet< เป็นครั้งแรก /2>**)**— เรานำคำว่า PLO มาใช้เพื่อหลีกเลี่ยงความสับสนที่เกี่ยวข้องกับคำในตลาดหุ้นแบบดั้งเดิม 'IPO' Karura จะใช้การสนับสนุนจาก KSM จากชุมชนเพื่อเข้าร่วมการประมูล Parachain KSM เหล่านี้จะถูกล็อคไว้ที่ Kusama และจะถูกส่งคืนให้กับผู้เข้าร่วมเมื่อสิ้นสุดการเช่าสล็อต parachain Karura จะ Paradrop โทเค็น KAR ดั้งเดิมให้กับผู้เข้าร่วม เป็นวิธีการกระจายโทเค็นไปยังผู้สนับสนุน Kusama & Karura ที่แท้จริง</p> 
  
  ![Image for post](https://miro.medium.com/max/1600/1*EtNqbSOXqs4ZkljaR0Db7Q.jpeg)</li> </ul> 
  
  

# **การอัพเดทระบบนิเวศ**

- Acala ได้รับเลือกให้เป็น DeFi Alliance เพื่อช่วยสนับสนุนสภาพคล่องของเครือข่ายสำหรับ DeFi Hub ของ Polkadot ([**Medium**](https://medium.com/acalanetwork/acala-selected-for-the-defi-alliance-accelerator-to-help-build-deploy-and-grow-the-defi-hub-of-c1526008963e)) โดยกลุ่มก่อนหน้านี้เป็นถึงเจ้าภาพทีม DeFi ชั้นนำบางทีมรวมถึง 0x, dYdX, Kyber Network, IDEX, Opyn, Set Protocol และ Synthetix

- เรายินดีต้อนรับผู้ทำงานร่วมกันเหล่านี้เข้าสู่โปรแกรมระบบนิเวศของ Acala: [Bifrost](http://bifrost.finance/) — โปรโตคอลสภาพคล่องแบบ cross-chain ที่จะรวม Acala Dollar (aUSD) เป็นโทเค็นสกุลเงินหลัก [Interlay](https://polkadot.network/bitcoin-is-coming-to-polkadot/?utm_content=142539261&utm_medium=social&utm_source=twitter&hss_channel=tw-1595615893) — Bitcoin ที่น่าเชื่อถือไปยังสะพาน Polkadot ซึ่งจะมีกรณีการใช้งานหลักประกันของ PolkaBTC, aUSD และ LDOT [Zenlink](https://www.zenlink.pro/) — โปรโตคอล DeX cross-chain ที่จะทำงานร่วมกันและผสานรวมกับ Acala

- Acala ได้ช่วยเปิดตัว [Substrate/Polkadot Developer Academy](http://.guru/polkadot-substrate) ([**tweet**](https://twitter.com/AcalaNetwork/status/1320921071835435008?s=20) **&** [**website**](http://ic.guru/polkadot-substrate))— หลักสูตร 6 สัปดาห์ + โครงการภาคปฏิบัติเพื่อเตรียม devs ที่มีประสบการณ์สำหรับอาชีพ Substrate / Polkadot หรือสตาร์ทอัพ โปรแกรมนี้พัฒนาโดยองค์กรฝึกอบรมด้านการพัฒนา MVP Studio ซึ่งเปิดตัวพร้อมกับ Parity และ Polkadot สอนโดย Bryan Chen ผู้ร่วมก่อตั้ง Acala/Laminar และรับรองโดย Dr. Gavin Wood ใครก็ตามที่จริงจังกับการสร้างบนสเปซของ Polkadot/Kusama/Substrate จะต้องตรวจสอบ [สิ่งนี้](http://ic.guru/polkadot-substrate) และ [tweet](https://twitter.com/AcalaNetwork/status/1320921071835435008?s=20) นี้ด้วย
  
  ![Image for post](https://miro.medium.com/max/5760/1*FajicLqehWMEzaUPx7ujjw.png)



# **อีเวนท์**

- At **Sub0 — Substrate Developer Conference**: Bryan Chen Co-Founder of Acala and Dan Forbes Dev Advocate at Parity showcased building a custom blockchain in under an hour. Watch the replay [here](https://t.co/XTLRKg8nZM?amp=1).

- **Polkadot’ Hello World! Gitcoin Challenge** is happening, check out the Acala Challenge [here](https://t.co/tzL4gpN5FJ?amp=1)

- Bette Chen, Co-Founder of Acala was on Outlier Venture’s Founders of Web3 Podcast — **Creating the DeFi Substrate for Polkadot**. Watch replay [here](https://www.youtube.com/watch?v=aueB19YH19g&list=UUd_K-AgiS2XV8_iuRQ7JyNQ).

- Ruitao Su, Co-Founder of Acala was on the **Crypto Tonight ‘Yes, Polkadot!’** panel alongside with Fabian Gompf from parity, Jack Platts from Hypersphere, Shiliang Tang from Ledger Prime. Watch replay [here](https://www.youtube.com/watch?v=xXgtpcf9NVE&feature=youtu.be).

- Acala is partaking in the 2020 Shanghai Blockchain Week as Hackathon sponsor and guest speaker. Register [here](https://www.eventbrite.com/e/the-6th-global-blockchain-summit-tickets-115473469255).

- Ruitao Su will speak at **Polkadot Decoded — the Polkadot Community Conference** **on Dec 3rd**, alongside with Dr Gavin Wood, Jutta Steiner, Camila Russo, Laura Shin + more TBA. Register [here](https://t.co/BWUXh8dwf2?amp=1)
  
  ![Image for post](https://miro.medium.com/max/1360/0*bb5Vh6rDQWQihkX0)



# Join Us

[Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launches on Polkadot and Kusama, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

[**Work with us.**](https://jobs.lever.co/acala/)



# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot that makes it fast and easy to use or build financial applications, improving trading efficiency and saving valuable time. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.
