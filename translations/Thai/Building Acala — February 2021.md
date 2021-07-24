# **การสร้าง Acala — กุมภาพันธ์ 2021 สรุป**

![Image for post](https://miro.medium.com/max/1600/1*oersbZPWGajTLHLnEkGbeQ.png)

กุมภาพันธ์นั้นเราทำได้ดีโดยนำชุมชน Polkadot และ Kusama เข้าใกล้ Parachain มากขึ้น แม้ว่าวันที่แน่นอนจะไม่ชัดเจน แต่เรา _สามารถ_ ยืนยันว่า Acala ยุ่งอยู่กับการทดสอบและปรับแต่งโค้ดบน Parachain testnet ของ Polkadot ในขณะที่เตรียมงานประมูล Karura Parachain ที่กำลังใกล้เข้ามาอย่างรวดเร็ว อย่าลืมเข้าร่วมรายการรอประมูลของ Karura Parachain เพื่อรับข้อมูลล่าสุดเกี่ยวกับงานและจองโบนัสผู้อ้างอิง 5% ให้กับคุณ และ 5% สำหรับทุกคนในเครือข่ายของคุณ

ในด้าน Acala เราเห็นความก้าวหน้าทางเทคนิคที่สำคัญบางอย่างในการถ่ายโอนโทเค็น cross-chain แรกของเราที่เสร็จสมบูรณ์ด้วย Plasm รวมถึงการเปิดตัว Acala EVM

เมื่อมองไปข้างหน้า สัปดาห์นี้เรารู้สึกตื่นเต้นที่จะเข้าร่วมคณะทำงานด้านเทคนิคของ Polkadot สำหรับ [DeFi Demo Day](https://www.crowdcast.io/e/defidemoday) ในวันพรุ่งนี้ (4 มีนาคม) เข้าร่วม Acala เพื่อรับการแนะนำและการสาธิตอย่างรวดเร็วจากทีม Parachain และทีมบริดจ์ พร้อมด้วยคณะผู้ดูแลโดย Cami Russo of the Defiant สำหรับ DeFi ที่มากขึ้น Acala จะเป็นเจ้าภาพในการท้าทายสองสามครั้งใน Chainlink hackathon ที่จะเกิดขึ้น อย่าลืมลงทะเบียนภายในวันที่ 15 มีนาคม เพื่อรับฟังจากโครงการชั้นนำใน crypto แข่งขันเพื่อชิงรางวัลมากกว่า 80,000 รายการ และเรียนรู้เกี่ยวกับโซลูชัน oracle แบบกระจายอำนาจล่าสุด เข้าร่วม ที่นี่: [https://chn.lk/3dAeB2I](https://chn.lk/3dAeB2I)

## **ธุรกรรมการส่งข้อความ cross-chain (XCMP) ที่ประสบความสำเร็จครั้งแรกบน Polkadot Testnet**

![Image for post](https://miro.medium.com/max/1400/0*j_NV5cE9SEQrMj-X)

Acala และ Plasm ทั้งสองทีมซึ่งวางแผนที่จะเป็น Parachain Polkadot และ Kusama ในอนาคตอันใกล้ ได้เชื่อมต่อผ่านเครือข่าย testnet Parachain ของ Polkadot และโอน cross-chain ของ Plasm's token (PLM) โดยใช้ฟังก์ชัน XCMP (การส่งข้อความ cross-chain) ตอนนี้เรามีการโอนย้ายโทเค็นแบบ cross-chain แล้ว เราเข้าใกล้ Kusama parachains ที่เริ่มใช้งานจริงอีกขั้น  เมื่อทีม Kusama ประกาศการเริ่มต้นของ crowdloans เครือข่าย Karura ของ Acala (ศูนย์กลาง DeFi ของ Kusama) จะเริ่มดำเนินการเพื่อโฮสต์ KSM งาน Crowdsourcing เพื่อเริ่มต้นเครือข่ายสำหรับการประมูลสล็อต Parachain  หลังจากงาน crowdsousrcing Karura จะเข้าร่วมการประมูลสล็อต Parachain  เมื่อชนะการประมูลครั้งนี้ Karura จะเปิดตัว mainnet

[ธุรกรรมการส่งข้อความ cross-chain (XCMP) ที่ประสบความสำเร็จครั้งแรกบน Polkadot Testnet](https://medium.com/acalanetwork/the-first-successful-cross-chain-messaging-passing-xcmp-transaction-on-polkadot-testnet-eb36af2ad8c3)

## **Acala เปิดตัว 'Acala EVM' สำหรับ DeFi บน Polkadot | ความเข้ากันได้ของ Ethereum กับฟังก์ชันของ Substrate แบบไม่จำกัด**

ทีมวิศวกรของ Acala ได้สร้างและเปิดตัว Acala EVM! เช่นเดียวกับ Ethereum ที่สามารถทำสิ่งต่าง ๆ ที่ Bitcoin ไม่สามารถทำได้ ซึ่งต่อมาได้สร้างแรงบันดาลใจให้กับนวัตกรรมใหม่ ๆ Substrate และ Polkadot นั้นแตกต่างอย่างสิ้นเชิงจาก Ethereum ในลักษณะที่จะเสริมพลังให้กับนวัตกรรมระดับเชนใหม่ ๆ นอก EVM sandbox เราเชื่อมั่นในพลังของ Substrate และได้สร้าง Acala EVM เพื่อปรับให้เหมาะสมสำหรับศักยภาพและอายุของ Substrate มากกว่าแค่ปรับใช้ Ethereum บน Polkadot

ฟีเจอร์เปลี่ยนเกมสองสามอย่างที่เปิดให้สำหรับผู้ใช้ DeFi และนักพัฒนาคือ “**Bring Your Own Gas**” ซึ่งอนุญาตให้ผู้ใช้จ่ายค่าธรรมเนียมแก๊สโดยโทเค็นแทบทุกชนิด และ **ตัวกำหนดตารางเวลาอัตโนมัติบนเครือข่าย< /0> ซึ่งเปิดใช้กรณีการใช้งาน เช่น การสมัครรับข้อมูลและการชำระเงินแบบประจำ ซึ่งไม่สามารถทำได้ด้วยแพลตฟอร์มบล็อกเชนแบบเดิม</p>

รายละเอียดเพิ่มเติมและลิงค์ที่นี่:

[Acala เปิดตัว 'Acala EVM' สำหรับ DeFi บน Polkadot | ความเข้ากันได้ของ Ethereum กับฟังก์ชันของ Substrate แบบไม่จำกัด...](https://medium.com/acalanetwork/acala-launches-the-acala-evm-for-defi-on-polkadot-ethereum-compatibility-with-unlimited-41aa893ca5a4)

## **ตัวอธิบาย: กระบวนการประมูล Parachain ทำงานอย่างไร**

Dan Reecer VP of Growth ของ Acala ได้รวบรวมหัวข้อ Twitter ที่อธิบายว่ากระบวนการประมูล Parachain ทำงานอย่างไร สิ่งนี้จะนำไปใช้กับทั้งการประมูล Karura และ Acala Parachain ที่จะเกิดขึ้น

## **การเริ่มต้นใช้งานโปรแกรม Acala Ambassador ได้เริ่มขึ้นแล้ว!**

โครงการ Acala Ambassador กำลังมีขึ้นและมีผู้เข้าร่วม 15 คนจากทั่วโลก Ambassador กำลังทำงานใน working group ดังต่อไปนี้:

- Translations และ Localization
- Content
- การดูแล Community
- อีเวนท์
- การพัฒนา & เทค

หากต้องการเข้าร่วมโปรแกรม Ambassador และเริ่มต้นการเริ่มต้นทำงาน [**สมัครที่นี่**](https://acala.hubspotpagebuilder.com/acala-ambassador-program)

## **Acala Community จีน**

Kelly, Yuzhu และทีมอื่นๆ ของเราในประเทศจีนกำลังทำงานเพื่อขยายแบรนด์ Acala และ Karura และสร้างการมีอยู่ของ community ในช่องต่างๆ เช่น WeChat เพื่อเริ่มต้นการเตรียมชุมชนชาวจีนสำหรับการประมูล Karura Parachain ที่จะเกิดขึ้น ทีมงานจะจัดงาน AMA ที่เน้น Karura ในสัปดาห์นี้ และจะสร้างกลุ่ม Karura WeChat กลุ่มแรกควบคู่กันไป ขณะนี้เรามีผู้คนมากกว่า 17,000 คนในบัญชีทางการของ Acala ในประเทศจีนและกลุ่ม Acala WeChat 13 กลุ่มที่เข้าถึงผู้คนมากกว่า 7,000 คน

## สมาชิกใหม่ในทีม

Alex Nechaiev ([LinkedIn](https://www.linkedin.com/in/alnech19/)) ร่วมงานกับเราในฐานะผู้จัดการผลิตภัณฑ์ด้านเทคนิคเพื่อทำงานอย่างใกล้ชิดกับทีมวิศวกรของเรา เขาทำงานร่วมกับเทคโนโลยีบล็อคเชนตั้งแต่ต้นปี 2017 Alex มีพื้นฐานเป็นนักพัฒนาและในการจัดการโครงการ โดยมี Substrate เป็นส่วนหนึ่งของพอร์ตโฟลิโอของเขา เขามีความกระตือรือร้นอย่างมากและอุทิศการทำงานให้กับเว็บ 3.0 และ Acala

## **อีเวนท์ที่กำลังจะมา**

- [**DeFi Demo Day**](https://www.crowdcast.io/e/defidemoday) — **วันพฤหัสบดีนี้** 4 มีนาคม (feat. Acala, Centrifuge, Interlay, Moonbeam, Phala, Plasm, Snowfork)
- [Chainlink hackathon](https://chainlink-2021.devpost.com/) — เริ่ม 15 มีนาคม
- เร็วๆ นี้: การประมูล Karura Parachain — [เรียนรู้เพิ่มเติม](https://medium.com/acalanetwork/karuras-approach-to-the-upcoming-parachain-lease-offering-plo-on-kusama-12fbf09ee463) หรือ [เข้าร่วมรายชื่อผู้รอ](https://forms.gle/1YShteaxrenxeauX8)
- เร็ว ๆ นี้: การประมูล Acala Parachain

## **👩‍💻👨‍💻 ลองใช้แอป Acala และ Karura DeFi บน testnet ก่อนที่เราจะเปิดใช้**

You can try the DeFi apps coming to the Polkadot and Kusama ecosystem by going to our [Getting Started guide](https://wiki.acala.network/learn/get-started) for instructions on getting testnet tokens, then using them at [apps.acala.network](http://apps.acala.network). Acala will provide DeFi to the Polkadot ecosystem, while Karura is serving the DeFi demand on the Kusama community.

_“What will I be able to do on Karura?”_

1.  Get Liquid KSM (LKSM) for your staked KSM. Your KSM continues to earn staking rewards, while you can use your LKSM in other yield-bearing uses such as liquidity providing.
2.  Make swaps on our AMM decentralized exchange
3.  Take out some kUSD stablecoins with your assets as collateral by initiating a collateralized debt position (CDP).
4.  Check out the [apps](http://apps.acala.network) for more…

![Image for post](https://miro.medium.com/max/3200/0*Zu0B8f4XoS5HVM-K)

We hope you have a great March, and see you on [Discord](https://discord.gg/vdbFVCH)!

![Image for post](https://miro.medium.com/max/2402/0*UgMpUJZXP3gBZubo.png)

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub and stablecoin of Polkadot that makes it fast and easy to use or build financial applications, improving trading efficiency and saving time. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities and robust security.

[Discord](https://discord.gg/vdbFVCH) | [Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc)
