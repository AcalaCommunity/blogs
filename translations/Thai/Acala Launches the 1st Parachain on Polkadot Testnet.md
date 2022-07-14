# Acala เปิดตัว Parachain ตัวแรกบน Polkadot Testnet

![รูปภาพจากโพส](https://miro.medium.com/max/8000/1*IGXwgFXEA7viM8upZgcw2g.jpeg)

เราได้บรรลุเป้าหมายสำคัญของพวกเราในการเปิดตัว Acala เป็น Parachain บน Polkadot — เราได้เปิดตัว Acala Mandala PC1 (Parachain Candidate 1) testnet เป็น parachain ตัวแรกใน [Rococo — Parachain testnet ของ Polkadot](https://medium.com/polkadot-network/introducing-rococo-polkadots-parachain-testnet-e3e67fc40b56)

Rococo ได้เปิดใช้งาน Parachain consensus และการรักษาความปลอดภัยที่ใช้ร่วมกันผ่าน [Cumulus](https://wiki.polkadot.network/docs/en/build-cumulus) รวมถึงการสื่อสารแบบ cross-chain ผ่าน HRMP (Horizontal Relay-chain Message Passing) HRMP ต้องการข้อความแบบ cross-chain ที่ถูกส่งผ่านโดย Relay-chains เพื่อเป็นแนวทางต่อการการสื่อสารจาก Parachain ไปยัง Parachain ผ่าน [XCMP](https://wiki.polkadot.network/docs/en/learn-crosschain) (Cross-chain Message Passing) ในภายหลัง

ด้วย Acala Mandala PC1 เราสามารถ

- **ทดสอบ DeFi แบบเต็มรูปแบบของ Acala** (stablecoin, stake Derivatives และ DeX) โดยใช้ข้อตกลงร่วมกันแบบ cross-chain และการส่งข้อความไปมา
- พัฒนางาน [Cross-Consensus Message (XCM) format](https://github.com/paritytech/xcm-format) ได้มากขึ้น และโดยเฉพาะเจาะจงไปที่ **มาตรฐานโทเค็นแบบ cross-chain ที่สามารถแทนกันได้** ซึ่งทางเราเป็นตัวตั้งตัวตี ตัวร่างของมาตรฐานอยู่ [ที่นี่](https://github.com/w3f/PSPs/blob/master/PSPs/drafts/psp-3.md) & การใช้งานพาเลท PoC อยู่ [ที่นี่](https://github.com/open-web3-stack/open-runtime-module-library/tree/rococo/xtokens)
- **ทดสอบโหนด Acala Collator** และพัฒนาระบบการให้รางวัล
- **ทดสอบการทำงานประสานกันของ cross-chain** **กับ Parachain อื่นๆ** เช่น Laminar, Plasm, Interlay และอื่นๆ
- พัฒนา **สะพานเชื่อม trustless staking ไปสู่ Relay-chain** ของโปรโตคอล Homa

# ชุมชนของนักพัฒนา Parachain

เราได้แบ่งปันสิ่งต่อไปนี้กับชุมชนนักพัฒนา Parachain

- **เปลี่ยน Substrate-based chain ให้กลายเป็น Parachain** นี้รวมถึงการเปลี่ยน nodes เป็น [Collators](https://wiki.polkadot.network/docs/en/maintain-collator) โดยการรวม Cumulus [ที่นี่](https://github.com/AcalaNetwork/Acala/pull/362)
- **การพัฒนาการโอนโทเค็นหลายๆตัวที่สามารถทดแทนกันได้แบบ cross-chain** — พาเลท 'xtoken' [ที่นี่](https://github.com/open-web3-stack/open-runtime-module-library/tree/rococo/xtokens) สิ่งเหล่านี้ได้ปลดล็อคทำให้สามารถถ่ายโอน ROC (โทเค็นเครือข่ายของ Rococo) ระหว่าง Rococo และ Mandala PC1 แล้ว; Parachains อื่น ๆ ที่นำสิ่งนี้ไปใช้หรือใช้มาตรฐานนี้ก็จะสามารถโอนโทเค็นให้กันได้

# อะไรต่อไป

สำหรับ Mandala PC1 จะรีเซ็ตโดยไม่มีการประกาศให้ทราบล่วงหน้าเพื่อให้ทันกับเวอร์ชันล่าสุดของ Rococo และนำเสนอฟังก์ชันใหม่ๆ และสนับสนุนการบูรณการกับ Parachains อื่นๆ การพัฒนาที่สำคัญสำหรับ Mandala Parachain Candidate Candidate คือ:

- **พัฒนา XCM Palette ต่อไป** พร้อมกับ Parity, Web3 Foundation และอื่นๆ ในชุมชนเพื่อให้พร้อมสำหรับการใช้งาน
- **เปิดใช้งาน Acala staking** พร้อมรางวัล/สแลชบนโหนด Acala Collator
- **การทดสอบการสื่อสารแบบ cross-chain อย่างครอบคลุม**กับ Parachains อื่นๆ และทำให้การใช้งานบางกรณีซึ่งพัฒนาแยกกันต่างหากเป็นไปได้ ตัวอย่างเช่น และส่ง aUSD ข้ามไปยัง Laminar เพื่อเป็นสกุลเงินหลักสำหรับการซื้อขายมาร์จิ้น และส่ง aUSD ข้ามไปสู่เครือข่าย Plasm เพื่อการชำระเงิน
- พร้อมเปิดตัว **การใช้งาน Homa staking Derivative (LDOT) Relay-chain bridge** เพื่อ trustless liquid staking สำหรับ Kusama และ Polkadot

# การเปิดตัว

นอกเหนือจาก Rococo และ Mandala แล้วทาง Acala จะเปิดตัวเครือข่าย Karura เป็น Parachain ตัวแรกบน Kusama เมื่อฟังก์ชัน Parachain เปิดใช้งานที่นั่น จากนั้นทางทีมจะเปิดตัว mainnet บน Polkadot Acala จะดำเนินการทั้งสองเครือข่าย — Karura & Acala mainnet เพื่อให้บริการโครงสร้างพื้นฐานของ DeFi และสภาพคล่องสำหรับทั้งระบบนิเวศ Kusama และ Polkadot จากนี้ไป เราจะเตรียมการสำหรับการประมูล Parachain เพื่อให้แน่ใจว่าเราจะได้พื้นที่ในการทำงานและเปิดตัวบนทั้งสองเครือข่าย **ติดตามได้** [**ที่นี่**](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) **เพื่อรับข้อมูลอัปเดตเกี่ยวกับการประมูลและการเปิดตัว Acala Parachain**

# เกี่ยวกับ Acala

[Acala](http://acala.network/) เป็นสมาคมการเงินแบบ decentralized แห่งแรกที่มีวิสัยทัศน์ในการสร้างความมั่นคงทางการเงิน สภาพคล่อง และการเข้าถึงได้ง่ายสำหรับบุคคลทั่วไป เครือข่าย Acala เป็นศูนย์กลางการเงินแบบ cross-chain สำหรับระบบนิเวศ Polkadot และอื่นๆ Acala ให้บริการด้วยโปรดักพื้นฐานทางการเงิน: เหรียญสเตเบิ้ลหลายๆตระกูลที่สามารถเป็นหลักประกันได้ ซึ่งได้รับการสนับสนุนจากสินทรัพย์แบบ cross-chain เช่น Bitcoin แล ะtrustless staking derivative และการแลกเปลี่ยนแบบ decentralized เพื่อปลดปล่อยสภาพคล่องและนวัตกรรมทางการเงินที่มีประสิทธิภาพ Acala เป็นแพลตฟอร์มแบบเปิดสำหรับ dApps ที่เน้นด้านการเงิน เพื่อนำไปใช้กับ smart contract หรือโปรโตคอลที่สร้างขึ้นมากับความสามารถที่ไม่ได้อยู่แต่ในกรอบแบบ cross-chain มีความปลอดภัย และการเพิ่มประสิทธิภาพทางการเงิน

**เข้าร่วมกับเรา**

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

![รูปภาพจากโพส](https://miro.medium.com/max/1500/0*YTeYSsHAVjOBCZu8.jpeg)

Acala ภาคภูมิใจที่เป็นผู้รับทุนจากมูลนิธิ Web3
