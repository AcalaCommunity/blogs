# ธุรกรรมการส่งข้อความ cross-chain (XCMP) ที่ประสบความสำเร็จครั้งแรกบน Polkadot Testnet

## Plasm Network & Acala ได้ทำธุรกรรม XCMP ครั้งแรกบนเครือข่าย testnet Rococo ของ Polkadot แล้ว

![รูปสำหรับโพสต์](https://miro.medium.com/max/2204/0*Bwnnq0OSWIc9dikX)

ในช่วงกลางคืน เราได้เป็นพยานพิเศษของประวัติศาสตร์คริปโตใน Polkadot.js และ telegram ระหว่างผู้พัฒนา Plasm Network และ Acala ทั้งสองทีมซึ่งวางแผนที่จะเป็น Parachain Polkadot และ Kusama ในอนาคตอันใกล้ ได้เชื่อมต่อผ่านเครือข่าย testnet Parachain ของ Polkadot และโอน cross-chain ของ Plasm's token (PLM) โดยใช้ฟังก์ชัน [XCMP](https://wiki.polkadot.network/docs/en/learn-crosschain) (การส่งข้อความ cross-chain) .

![รูปสำหรับโพสต์](https://miro.medium.com/max/1880/0*_PHpXfxScO1sDNs_)

## **เรามาที่นี่ได้อย่างไร **

Acala สร้างพาเลท xtoken ([github](https://github.com/open-web3-stack/open-runtime-module-library/tree/sw/rococo-v1/xtokens)) Substrate ซึ่งสร้างขึ้นสำหรับการถ่ายโอนโทเค็นข้ามสายโซ่ภายในระบบนิเวศ Polkadot และ Kusama ตั้งแต่นั้นเป็นต้นมา เราได้เปิดแหล่งที่มาของพาเลทนี้ และทำให้มันเป็น 'สินค้าทั่วไป' สำหรับ Parachain ใด ๆ ที่จะรวมเข้ากับโครงการของพวกเขา นอกจากนี้เรายังสร้างการถ่ายโอนโทเค็น cross-chain ระหว่าง Acala testnet และ Laminar testnet ด้วยข้อความ cross-chain ได้สำเร็จ

116 / 5000 ผลลัพธ์การแปล ระหว่างการทดสอบ [Aleksandr Krupenkin](https://github.com/akru) หัวหน้าวิศวกรของ Plasm Network พบปัญหาบางอย่างเกี่ยวกับการใช้ XCM บน Rococo  Aleksandr แก้ไขปัญหาและ [pull request ของเขาถูกรวมโดย Parity](https://github.com/paritytech/cumulus/pull/309)

สุดท้าย หลังจากที่การเปลี่ยนแปลงได้รับการยอมรับและ XCM ทำงานอย่างถูกต้อง Parachains ทั้งสองได้เสร็จสิ้นการถ่ายโอนโทเค็น cross-chain ที่ประสบความสำเร็จ ซึ่งคุณสามารถดูได้ในวิดีโอนี้:

## **ขั้นตอนต่อไปสำหรับการประมูล parachain Acala & Karura และการเปิดตัว **

ตอนนี้เรามีการโอนย้ายโทเค็นแบบ cross-chain แล้ว เราเข้าใกล้ Kusama parachains ที่เริ่มใช้งานจริงอีกขั้น  เมื่อทีม Kusama ประกาศการเริ่มต้นของ crowdloans เครือข่าย Karura ของ Acala (ศูนย์กลาง DeFi ของ Kusama) จะเริ่มดำเนินการเพื่อโฮสต์ KSM [งาน Crowdsourcing](http://acala.network/karura-crowdloan) เพื่อเริ่มต้นเครือข่ายสำหรับการประมูลสล็อต Parachain  หลังจากงาน crowdsousrcing Karura จะเข้าร่วมการประมูลสล็อต Parachain  เมื่อชนะการประมูลครั้งนี้ Karura จะเปิดตัว mainnet 175 / 5000 ผลลัพธ์การแปล **ในการเข้าร่วมกับคนอื่นๆ อีก 19,000 คนในการประมูลของ Karura Parachain และมีสิทธิ์ได้รับโบนัส KAR 10% แบ่งระหว่างคุณและกรรมการของคุณ** [**ลงทะเบียนที่นี่**](https://forms.gle/Qj8i2RxG3fHyg8DA8)30>.</strong> 0>

กระบวนการประมูลของ Parachain ทำงานอย่างไร?  ดูที่นี่:

หลังจากการประมูล Parachain ของ Karura การประมูล crowdloan จาก Polkadot และการประมูล Parachain จะเริ่มเกิดขึ้น  Acala จะจัดงาน Crowdsourcing อีกครั้ง คราวนี้สำหรับ DOT และจากนั้นจะใช้ภาชนะ DOT นี้เพื่อเข้าร่วมในการประมูล Parachain Polkadot ครั้งแรก  หลังจากชนะการประมูล Acala จะเปิดตัว mainnet

![รูปสำหรับโพสต์](https://miro.medium.com/max/2402/0*4QUW9GSAV2UxUI6E.png)

# เกี่ยวกับ Acala

[Acala](http://acala.network/) เป็นศูนย์กลางทางการเงินแบบกระจายอำนาจของ Polkadot ที่ทำให้ใช้งานหรือสร้างแอปพลิเคชันทางการเงินได้อย่างรวดเร็วและง่ายดาย เพิ่มประสิทธิภาพการเทรดและประหยัดเวลา แพลตฟอร์มนำเสนอชุดพื้นฐานทางการเงิน: stablecoin ค้ำประกันที่มีความหลากหลายซึ่งได้รับการสนับสนุนจากทรัพย์สิน cross-chain เช่น Bitcoin อนุพันธ์ trustless staking และการแลกเปลี่ยนแบบกระจายอำนาจเพื่อปลดปล่อยสภาพคล่องและนวัตกรรมทางการเงินที่มีอำนาจ Acala เป็นแพลตฟอร์มที่เข้ากันได้กับ Ethereum สำหรับแอปพลิเคชันทางการเงินเพื่อใช้ smart contract หรือโปรโตคอลในตัวพร้อมความสามารถ cross-chain ที่พร้อมใช้งานทันทีและการรักษาความปลอดภัยที่แข็งแกร่ง

[Discord](https://discord.gg/vdbFVCH) | [Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki)

# เกี่ยวกับ Plasm

Plasm Network เป็นแพลตฟอร์มสัญญาอัจฉริยะที่ปรับขนาดได้บน Polkadot ซึ่งสนับสนุนโซลูชันเลเยอร์ 2 ที่ทันสมัยและ Ethereum Virtual Machine  ผลลัพธ์การแปล มันถูกสร้างขึ้นบน Substrate และได้รับการออกแบบให้เป็น Polkadot Parachain  Plasm Network มุ่งเน้นไปที่การสร้างแพลตฟอร์ม smart contract ที่ยอดเยี่ยม เพื่อให้นักพัฒนา dApps บน Polkadot ไม่จำเป็นต้องให้ความสนใจกับโครงสร้างพื้นฐานมากนัก และสามารถมุ่งเน้นไปที่ dApps ของตนได้มากขึ้น ตามหลักการแล้ว นักพัฒนาสามารถสร้างแอพพลิเคชั่นอะไรก็ได้บน Plasm Network โดยไม่ต้องคำนึงถึงความสามารถในการปรับขนาดของมัน

[Website](https://www.plasmnet.io/) | [Twitter](https://twitter.com/Plasm_Network) | [Telegram](https://t.me/PlasmOfficial) | [Discord](https://discord.gg/Z3nC9U4) | [GitHub](https://github.com/PlasmNetwork/Plasm)
