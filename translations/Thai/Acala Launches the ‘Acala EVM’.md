# **Acala เปิดตัว 'Acala EVM' สำหรับ DeFi บน Polkadot | ความเข้ากันได้ของ Ethereum กับฟังก์ชันของ Substrate แบบไม่จำกัด**

![Image for post](https://miro.medium.com/max/6000/1*FNYYia98MytjFEU1Dtuzqw.png)

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

หากคุณยังใหม่กับที่นี่ Acala เป็นแพลตฟอร์มการเงินแบบกระจายอำนาจ (DeFi) ที่เข้ากันได้กับ Ethereum ที่สร้างขึ้นสำหรับการปรับขนาด โดยใช้ประโยชน์จากเครือข่าย cross-chain ของ Polkadot แม้ว่า Acala จะเป็น Parachain ที่ให้บริการโครงสร้างพื้นฐานเลเยอร์ 1 แต่ทีม Acala ได้สร้างเลเยอร์แอปพลิเคชันทั้งหมดไว้บน Parachain Acala’s applications are built around a stable asset (aUSD) and offers end-user applications such as borrowing, lending, synthetic asset trading, and interest earning, all executed extremely fast with inexpensive gas fees. Developers can also leverage Acala as a platform on which to build their own applications.

The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange. **Overall, Acala’s platform also offers:**

1.  **Micro Gas Fees** — Acala solves the gas fee problem for DeFi users, in combination with the ability to ‘bring your own gas’ as mentioned above
2.  **Staking derivative L-DOT** (Liquid DOT to release liquidity from staked DOT for use in Acala’s DeFi applications)
3.  **Stablecoin borrowing and lending** (DOT, Bitcoin and L-DOT used as primary collateral asset)
4.  **Earning yield and interest**
5.  Trading on **decentralized exchange** (DEX)
6.  On-chain **governance**
7.  On-chain **Treasury**
8.  Native network of **aggregated oracle price feeds**
9.  **On-chain sovereign wealth fund** to sustain the network’s future ([read more](https://medium.com/acalanetwork/building-a-decentralized-sovereign-wealth-fund-6a5a0ae995b1))
10. **Continuously upgrade with no forks**: Keep in mind that Acala can upgrade seamlessly with no forks. This means that the future is virtually limitless. Any new Substrate pallet (a product or feature in the form of a DeFi primitive or runtime) can smoothly integrate into Acala. It’s like getting an iPhone 12 that will auto-upgrade to a 13, 14, 15+ in the palm of your hand.

![Image for post](https://miro.medium.com/max/3200/0*iHVQdZllz1MxLwuy)

http://apps.acala.network

Thanks for checking out the new Acala EVM. We’ll continue to keep you updated on the progress of the Acala EVM, as well as further educational material on the different benefits it provides to the ecosystem. As always, you can find us on [Discord](https://discord.gg/vdbFVCH), [subscribe to our newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) for updates, or any of our channels below:

![Image for post](https://miro.medium.com/max/2402/0*BvF8sTfeQd4Sc71D.png)

# **About Acala**

[Acala](http://acala.network/) is the decentralized financial hub and stablecoin of Polkadot that makes it fast and easy to use or build financial applications, improving trading efficiency and saving time. The platform, operated by micro gas fees, offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities and robust security.

[Discord](https://discord.gg/vdbFVCH) | [Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) | [All Channels](https://linktr.ee/acalanetwork)
