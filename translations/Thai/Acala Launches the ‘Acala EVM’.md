# **Acala เปิดตัว 'Acala EVM' สำหรับ DeFi บน Polkadot | ความเข้ากันได้ของ Ethereum กับฟังก์ชันของ Substrate แบบไม่จำกัด**

![รูปสำหรับโพสต์](https://miro.medium.com/max/6000/1*FNYYia98MytjFEU1Dtuzqw.png)

## Acala EVM ใช้ประโยชน์จาก Ethereum ที่ดีที่สุดในขณะที่ปลดล็อกศักยภาพของ Substrate ด้วยความสามารถการประกอบได้, กระเป๋าเดี่ยว, ประสบการณ์ Acala-EVM-Substrate-WASM พร้อมกับ 'นำแก๊สของคุณมาเอง', การตั้งเวลาอัตโนมัติบนเชนและอื่น ๆ

ทีมวิศวกรของ Acala ได้สร้างและเปิดตัว Acala EVM! นวัตกรรมนี้เป็นนวัตกรรมใหม่สำหรับระบบนิเวศ Polkadot ทำให้ Acala สามารถมอบประสบการณ์การใช้งานแบบฟูลสแตก (Acala+EVM+Substrate+WASM) ให้กับนักพัฒนา Solidity, Substrate และ Web3 ได้อย่างราบรื่นด้วยกระเป๋าเงินเดียว Acala EVM ยังนำความสามารถในการบีบอัดโปรโตคอลสำหรับรันไทม์ EVM และ Substrate (หรือที่เรียกว่าพาเลท) และช่วยให้นักพัฒนาสามารถสร้างและปรับใช้ DApps บน Acala ด้วยซัพพอร์ทเครื่องมือที่ยอดเยี่ยม

เช่นเดียวกับ Ethereum ที่สามารถทำสิ่งต่าง ๆ ที่ Bitcoin ไม่สามารถทำได้ ซึ่งต่อมาได้สร้างแรงบันดาลใจให้กับนวัตกรรมใหม่ ๆ Substrate และ Polkadot นั้นแตกต่างอย่างสิ้นเชิงจาก Ethereum ในลักษณะที่จะเสริมพลังให้กับนวัตกรรมระดับเชนใหม่ ๆ นอก EVM sandbox เราเชื่อมั่นในพลังของ Substrate และได้สร้าง Acala EVM เพื่อปรับให้เหมาะสมสำหรับศักยภาพและอายุของ Substrate มากกว่าแค่ปรับใช้ Ethereum บน Polkadot

# **The Acala EVM**

## **สภาพแวดล้อม DeFi ที่ประกอบได้**

Smart Contract Dapps ที่ปรับใช้ใน Acala EVM สามารถใช้สินทรัพย์ดั้งเดิมและ cross-chain เช่น DOT, ACA, aUSD, renBTC, XBTC และอื่นๆ โทเค็น ERC-20 ที่ปรับใช้ใน EVM ยังสามารถให้บริการที่ระดับรันไทม์ เพื่อแสดงรายการใน DEX หรือ (โดยการอนุมัติจาก governance) เพื่อใช้เป็นโทเค็นค่าธรรมเนียมแก๊ส ซึ่งหมายความว่า ตัวอย่างเช่น เพื่อนของเราที่ Ampleforth สามารถปรับใช้คอนแทรค AMPL บน Acala EVM เพื่อให้พร้อมใช้งานเป็นโทเค็นดั้งเดิม ดังนั้นจึงสามารถใช้เพื่อชำระค่าธรรมเนียมการทำธุรกรรมและแสดงรายการโดยตรงบน DEX ของเรา

ยังใหม่กับแนวคิดเรื่องความสามารถในการประกอบได้? A16z ทำได้ดีมากใน [4 Eras of Blockchain Computing: Degrees of Composability](https://a16z.com/2018/12/16/4-eras-of-blockchain-computing-degrees-of-composability/#:~:text=A%20platform%20is%20composable%20if,more%20rapid%20and%20compounding%20innovation.)

เพื่อให้สิ่งนี้ 'เป็นจริง' มากขึ้น โปรดดูด้านล่างในฐานะผู้ร่วมก่อตั้งและซีทีโอของ Acala เมื่อเร็ว ๆ นี้ Bryan Chen สาธิตกรณีการใช้งานของ Acala EVM เมื่อเขาปรับใช้ Uniswap บน Acala และดำเนินการซื้อขายภายใน 2 นาที:

## **DeFi ดั้งเดิมอื่นๆที่ประกอบได้อย่างสมบูรณ์ ใน Acala EVM**

- **นำแก๊สมาเอง**: เพิ่มความสามารถให้กับการทำธุรกรรมกับโทเค็นใด ๆ — โทเค็นดั้งเดิมและโทเค็นแบบ cross-chain ที่รวมเข้ากับ Acala จะสามารถใช้จ่ายแก๊สได้ เมื่อมันทำงาน อาจมีลักษณะดังนี้: _คุณกำลังส่ง wrapped ETH ไปยัง Acala เพื่อเริ่มใช้งานใน DeFi หรือไม่ ส่ง ETH ของคุณไปยัง Acala ผ่านการบริดจ์ และเริ่มปรับใช้ wrapped ETH ทันทีในแอป Acala DeFi โดยใช้ wrapped ETH เป็นค่าธรรมเนียมแก๊ส ไม่ต้องไปหา ACA จากที่ไหน_
- **ตัวกำหนดตารางเวลาอัตโนมัติในเครือข่าย** ที่เปิดใช้งานกรณีการใช้งาน เช่น การสมัครรับข้อมูลและการชำระเงินแบบประจำ ลองใช้ [ที่นี่](https://wiki.acala.network/build/development-guide/smart-contracts/advanced/use-on-chain-scheduler) หรือดูการสาธิต 6 นาทีด้านล่าง

- **Native และ cross-chain token** มีอยู่ใน ERC20: DOT, ACA, aUSD, XBTC (จาก ChainX), LDOT (การ stake สภาพคล่องของ DOT), RENBTC และอื่นๆ
- เครือข่าย oracles เพื่อรับฟีดราคา ลอง [ที่นี่](https://wiki.acala.network/build/development-guide/smart-contracts/advanced/use-oracle-feeds)
- โปรโตคอล เช่น DEX การให้กู้ยืม stablecoin และอนุพันธ์การ stake สภาพคล่อง (เช่น สภาพคล่อง DOT สำหรับ DOT ที่คุณ stake)

## **🐰🕳 ถ้าอยากลงลึกเกี่ยวกับ Acala EVM โปรดดูที่** [**ส่วน EVM เชิงลึกของ Acala Wiki**](https://wiki.acala.network/learn/basics/acala-evm/acala-evm-composable-defi-stack)**.**

## ทดลองใช้งาน ETHDenver 2021

Acala กำลังเปิดตัว Acala EVM ที่ ETHDenver 2021 โดยเสนอ $3k USD สำหรับแฮกเกอร์เพื่อ “**สร้าง DApp โดยใช้ Acala EVM**” หรือ “**สร้าง DApp โดยใช้ Acala EVM ด้วยฟังก์ชันตัวกำหนดเวลาอัตโนมัติแบบ on-Chain**”

- ค้นหา [**คู่มือแฮ็กเกอร์ EHDenver**](https://wiki.acala.network/general/contribution-rewards/ethdenver-hacker)** ของ Acala**
- ดู [**ETHDenver's Bounty Hub**](https://www.ethdenver.com/post/acala) และ [**แนวทางของทีม**](https://www.ethdenver.com/judging)****

[สร้าง DeFi DApp Polkadot ของคุณพร้อมด้วย EVM ของ Acala ที่ EHDenver 2021](https://medium.com/acalanetwork/make-your-defi-dapp-polkadot-ready-with-acalas-evm-at-ethdenver-2021-b542090f6af1)

# **Acala ในระดับสูง**

หากคุณยังใหม่กับที่นี่ Acala เป็นแพลตฟอร์มการเงินแบบกระจายอำนาจ (DeFi) ที่เข้ากันได้กับ Ethereum ที่สร้างขึ้นสำหรับการปรับขนาด โดยใช้ประโยชน์จากเครือข่าย cross-chain ของ Polkadot แม้ว่า Acala จะเป็น Parachain ที่ให้บริการโครงสร้างพื้นฐานเลเยอร์ 1 แต่ทีม Acala ได้สร้างเลเยอร์แอปพลิเคชันทั้งหมดไว้บน Parachain แอปพลิเคชันของ Acala สร้างขึ้นจากสินทรัพย์ stable (aUSD) และนำเสนอแอปพลิเคชันสำหรับผู้ใช้ปลายทาง เช่น การยืม การให้ยืม การซื้อขายสินทรัพย์สังเคราะห์ และการรับดอกเบี้ย ทั้งหมดนี้ดำเนินการอย่างรวดเร็วโดยมีค่าธรรมเนียมแก๊สที่ไม่แพง นักพัฒนายังสามารถใช้ประโยชน์จาก Acala เป็นแพลตฟอร์มสำหรับสร้างแอปพลิเคชันของตนเอง

แพลตฟอร์มนำเสนอชุดของพื้นฐานทางการเงิน: stablecoin หลายหลักประกันซึ่งได้รับการสนับสนุนจากสินทรัพย์ cross-chain เช่น Bitcoin อนุพันธ์การ stake แบบ trustless และการแลกเปลี่ยนแบบกระจายอำนาจ **โดยรวมแล้ว แพลตฟอร์มของ Acala ยังมี:**

1.  **ค่าธรรมเนียม Micro Gas** — Acala แก้ปัญหาค่าธรรมเนียมแก๊สสำหรับผู้ใช้ DeFi ร่วมกับความสามารถในการ "นำแก๊สมาเอง" ตามที่กล่าวไว้ข้างต้น
2.  **Stake Derivative L-DOT** (Liquid DOT เพื่อปลดปล่อยสภาพคล่องจาก Stake DOT สำหรับใช้ในแอปพลิเคชัน DeFi ของ Acala)
3.  **การยืมและให้ยืม Stablecoin** (DOT, Bitcoin และ L-DOT ใช้เป็นหลักทรัพย์ค้ำประกันหลัก)
4.  **รับผลตอบแทนและดอกเบี้ย**
5.  เทรดบน **decentralized exchange** (DEX)
6.  On-chain **governance**
7.  On-chain **Treasury**
8.  เครือข่ายเนทีฟของ **ฟีดราคา Oracle ที่รวบรวมไว้**
9.  **กองทุนความมั่งคั่งแบบ On-chain** เพื่อรักษาอนาคตของเครือข่าย ([อ่านเพิ่มเติม](https://medium.com/acalanetwork/building-a-decentralized-sovereign-wealth-fund-6a5a0ae995b1))
10. **อัปเกรดอย่างต่อเนื่องโดยไม่ต้อง fork**: โปรดทราบว่า Acala สามารถอัปเกรดได้อย่างราบรื่นโดยไม่ต้อง fork ซึ่งหมายความว่าอนาคตแทบจะไร้ขีดจำกัด พาเลท Substrate ใหม่ใดๆ (ผลิตภัณฑ์หรือคุณลักษณะในรูปแบบของ DeFi ดั้งเดิมหรือรันไทม์) สามารถรวมเข้ากับ Acala ได้อย่างราบรื่น เหมือนกับได้ iPhone 12 ที่จะอัปเกรดอัตโนมัติเป็น 13, 14, 15+ ในมือคุณ

![รูปสำหรับโพสต์](https://miro.medium.com/max/3200/0*iHVQdZllz1MxLwuy)

http://apps.acala.network

ขอบคุณที่รับชม Acala EVM ใหม่ เราจะแจ้งความคืบหน้าให้คุณทราบเกี่ยวกับความคืบหน้าของ Acala EVM ตลอดจนเอกสารการศึกษาเพิ่มเติมเกี่ยวกับประโยชน์ต่างๆ ที่มอบให้กับระบบนิเวศ เช่นเคย คุณสามารถพบเราได้ที่ [Discord](https://discord.gg/vdbFVCH), [สมัครรับจดหมายข่าวของเรา](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc)เพื่อรับข้อมูลอัปเดต หรือช่องใดๆ ของเราด้านล่าง:

![รูปสำหรับโพสต์](https://miro.medium.com/max/2402/0*BvF8sTfeQd4Sc71D.png)

# **เกี่ยวกับ Acala**

[Acala](http://acala.network/) เป็นศูนย์กลางทางการเงินแบบกระจายอำนาจของ Polkadot ที่ทำให้ใช้งานหรือสร้างแอปพลิเคชันทางการเงินได้อย่างรวดเร็วและง่ายดาย เพิ่มประสิทธิภาพการเทรดและประหยัดเวลา แพลตฟอร์มที่ดำเนินการด้วยค่าธรรมเนียมแก๊สเพียงเล็กน้อย: stablecoin ค้ำประกันที่มีความหลากหลายซึ่งได้รับการสนับสนุนจากทรัพย์สิน cross-chain เช่น Bitcoin อนุพันธ์ trustless staking และการแลกเปลี่ยนแบบกระจายอำนาจเพื่อปลดปล่อยสภาพคล่องและนวัตกรรมทางการเงินที่มีอำนาจ Acala เป็นแพลตฟอร์มที่เข้ากันได้กับ Ethereum สำหรับแอปพลิเคชันทางการเงินเพื่อใช้ smart contract หรือโปรโตคอลในตัวพร้อมความสามารถ cross-chain ที่พร้อมใช้งานทันทีและการรักษาความปลอดภัยที่แข็งแกร่ง

[Discord](https://discord.gg/vdbFVCH) | [Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) | [All Channels](https://linktr.ee/acalanetwork)
