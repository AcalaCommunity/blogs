# ธุรกรรมการส่งข้อความ cross-chain (XCMP) ที่ประสบความสำเร็จครั้งแรกบน Polkadot Testnet

## Plasm Network & Acala ได้ทำธุรกรรม XCMP ครั้งแรกบนเครือข่าย testnet Rococo ของ Polkadot แล้ว

![Image for post](https://miro.medium.com/max/2204/0*Bwnnq0OSWIc9dikX)

ในช่วงกลางคืน เราได้เป็นพยานพิเศษของประวัติศาสตร์คริปโตใน Polkadot.js และ telegram ระหว่างผู้พัฒนา Plasm Network และ Acala ทั้งสองทีมซึ่งวางแผนที่จะเป็น Parachain Polkadot และ Kusama ในอนาคตอันใกล้ ได้เชื่อมต่อผ่านเครือข่าย testnet Parachain ของ Polkadot และโอน cross-chain ของ Plasm's token (PLM) โดยใช้ฟังก์ชัน [XCMP](https://wiki.polkadot.network/docs/en/learn-crosschain) (การส่งข้อความ cross-chain) .

![Image for post](https://miro.medium.com/max/1880/0*_PHpXfxScO1sDNs_)

## **เรามาที่นี่ได้อย่างไร **

Acala สร้างพาเลท xtoken ([github](https://github.com/open-web3-stack/open-runtime-module-library/tree/sw/rococo-v1/xtokens)) Substrate ซึ่งสร้างขึ้นสำหรับการถ่ายโอนโทเค็นข้ามสายโซ่ภายในระบบนิเวศ Polkadot และ Kusama ตั้งแต่นั้นเป็นต้นมา เราได้เปิดแหล่งที่มาของพาเลทนี้ และทำให้มันเป็น 'สินค้าทั่วไป' สำหรับ Parachain ใด ๆ ที่จะรวมเข้ากับโครงการของพวกเขา นอกจากนี้เรายังสร้างการถ่ายโอนโทเค็น cross-chain ระหว่าง Acala testnet และ Laminar testnet ด้วยข้อความ cross-chain ได้สำเร็จ

116 / 5000 ผลลัพธ์การแปล ระหว่างการทดสอบ [Aleksandr Krupenkin](https://github.com/akru) หัวหน้าวิศวกรของ Plasm Network พบปัญหาบางอย่างเกี่ยวกับการใช้ XCM บน Rococo  Aleksandr แก้ไขปัญหาและ [pull request ของเขาถูกรวมโดย Parity](https://github.com/paritytech/cumulus/pull/309)

สุดท้าย หลังจากที่การเปลี่ยนแปลงได้รับการยอมรับและ XCM ทำงานอย่างถูกต้อง Parachains ทั้งสองได้เสร็จสิ้นการถ่ายโอนโทเค็น cross-chain ที่ประสบความสำเร็จ ซึ่งคุณสามารถดูได้ในวิดีโอนี้:

## **ขั้นตอนต่อไปสำหรับการประมูล parachain Acala & Karura และการเปิดตัว **

Now that we have completed a cross-chain token transfer, we are one step closer to Kusama parachains starting to go live. Once the Kusama team announces the beginning of crowdloans, Acala’s Karura network (the DeFi hub of Kusama) will begin it’s process to host a KSM [crowdsourcing event](http://acala.network/karura-crowdloan) to bootstrap the network for the parachain slot auction. After the crowdsousrcing event, Karura will participate in the parachain slot auction. Upon winning this auction, Karura will then launch its mainnet. **To join the 19,000 other people on Karura Parachain Auction Waitlist and be eligible for a 10% KAR bonus split between you and your referee,** [**sign up here**](https://forms.gle/Qj8i2RxG3fHyg8DA8)**.**

How does the parachain auction process work? Watch here:

After Karura’s parachain auction, Polkadot-based crowdloans and parachain auctions will begin to happen. Acala will host another crowdsourcing event, this time for DOT, and will then use this pot of DOT to participate in the first Polkadot parachain auction. After winning an auction, Acala will then launch its mainnet.

![Image for post](https://miro.medium.com/max/2402/0*4QUW9GSAV2UxUI6E.png)

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub and stablecoin of Polkadot that makes it fast and easy to use or build financial applications, improving trading efficiency and saving time. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de-facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities and robust security.

[Discord](https://discord.gg/vdbFVCH) | [Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki)

# About Plasm

Plasm Network is a scalable smart contract platform on Polkadot supporting cutting edge layer 2 solutions and Ethereum Virtual Machine. It is built on Substrate and designed to be a Polkadot Parachain. Plasm Network focuses on making a great smart contract platform so that dApps developers on Polkadot do not need to pay much attention to infrastructure and can focus more on their dApps. Ideally, the developers can build whatever applications on Plasm Network without having to consider its scalability.

[Website](https://www.plasmnet.io/) | [Twitter](https://twitter.com/Plasm_Network) | [Telegram](https://t.me/PlasmOfficial) | [Discord](https://discord.gg/Z3nC9U4) | [GitHub](https://github.com/PlasmNetwork/Plasm)
