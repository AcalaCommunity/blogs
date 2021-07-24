# **การสร้าง Acala — กุมภาพันธ์ 2021 สรุป**

![รูปสำหรับโพสต์](https://miro.medium.com/max/1600/1*oersbZPWGajTLHLnEkGbeQ.png)

กุมภาพันธ์นั้นเราทำได้ดีโดยนำชุมชน Polkadot และ Kusama เข้าใกล้ Parachain มากขึ้น แม้ว่าวันที่แน่นอนจะไม่ชัดเจน แต่เรา _สามารถ_ ยืนยันว่า Acala ยุ่งอยู่กับการทดสอบและปรับแต่งโค้ดบน Parachain testnet ของ Polkadot ในขณะที่เตรียมงานประมูล Karura Parachain ที่กำลังใกล้เข้ามาอย่างรวดเร็ว อย่าลืมเข้าร่วมรายการรอประมูลของ Karura Parachain เพื่อรับข้อมูลล่าสุดเกี่ยวกับงานและจองโบนัสผู้อ้างอิง 5% ให้กับคุณ และ 5% สำหรับทุกคนในเครือข่ายของคุณ

ในด้าน Acala เราเห็นความก้าวหน้าทางเทคนิคที่สำคัญบางอย่างในการถ่ายโอนโทเค็น cross-chain แรกของเราที่เสร็จสมบูรณ์ด้วย Plasm รวมถึงการเปิดตัว Acala EVM

เมื่อมองไปข้างหน้า สัปดาห์นี้เรารู้สึกตื่นเต้นที่จะเข้าร่วมคณะทำงานด้านเทคนิคของ Polkadot สำหรับ [DeFi Demo Day](https://www.crowdcast.io/e/defidemoday) ในวันพรุ่งนี้ (4 มีนาคม) เข้าร่วม Acala เพื่อรับการแนะนำและการสาธิตอย่างรวดเร็วจากทีม Parachain และทีมบริดจ์ พร้อมด้วยคณะผู้ดูแลโดย Cami Russo of the Defiant สำหรับ DeFi ที่มากขึ้น Acala จะเป็นเจ้าภาพในการท้าทายสองสามครั้งใน Chainlink hackathon ที่จะเกิดขึ้น อย่าลืมลงทะเบียนภายในวันที่ 15 มีนาคม เพื่อรับฟังจากโครงการชั้นนำใน crypto แข่งขันเพื่อชิงรางวัลมากกว่า 80,000 รายการ และเรียนรู้เกี่ยวกับโซลูชัน oracle แบบกระจายอำนาจล่าสุด เข้าร่วม ที่นี่: [https://chn.lk/3dAeB2I](https://chn.lk/3dAeB2I)

## **ธุรกรรมการส่งข้อความ cross-chain (XCMP) ที่ประสบความสำเร็จครั้งแรกบน Polkadot Testnet**

![รูปสำหรับโพสต์](https://miro.medium.com/max/1400/0*j_NV5cE9SEQrMj-X)

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

คุณลองใช้แอป DeFi ที่เข้ามาในระบบนิเวศ Polkadot และ Kusama ได้โดยไปที่[คู่มือเริ่มต้นใช้งาน](https://wiki.acala.network/learn/get-started)เพื่อดูคำแนะนำในการรับโทเค็น testnet จากนั้นใช้ที่ [apps.acala.network](http://apps.acala.network) Acala จะให้บริการ DeFi แก่ระบบนิเวศ Polkadot ในขณะที่ Karura ตอบสนองความต้องการ DeFi ในชุมชน Kusama

_“ฉันจะทำอะไรกับ Karura ได้บ้าง”_

1.  รับ Liquid KSM (LKSM) สำหรับ KSM ที่คุณ stake ไว้ KSM ของคุณยังคงได้รับรางวัลการ stake ในขณะที่คุณสามารถใช้ LKSM ของคุณในการใช้งานที่ให้ผลตอบแทนอื่นๆ เช่น การจัดหาสภาพคล่อง
2.  ทำการแลกเปลี่ยนใน exchange แบบกระจายอำนาจ AMM ของเรา
3.  นำ kUSD ที่มีเสถียรภาพออกมาพร้อมกับสินทรัพย์ของคุณเป็นหลักประกันโดยการเริ่มต้นสถานะหนี้ที่มีหลักประกัน (CDP)
4.  ตรวจสอบ [แอป](http://apps.acala.network) สำหรับข้อมูลเพิ่มเติม...

![รูปสำหรับโพสต์](https://miro.medium.com/max/3200/0*Zu0B8f4XoS5HVM-K)

เราหวังว่าคุณจะมีเดือนมีนาคมที่ยอดเยี่ยม แล้วพบกันที่ [Discord](https://discord.gg/vdbFVCH)!

![รูปสำหรับโพสต์](https://miro.medium.com/max/2402/0*UgMpUJZXP3gBZubo.png)

# เกี่ยวกับ Acala

[Acala](http://acala.network/) เป็นศูนย์กลางทางการเงินแบบกระจายอำนาจของ Polkadot ที่ทำให้ใช้งานหรือสร้างแอปพลิเคชันทางการเงินได้อย่างรวดเร็วและง่ายดาย เพิ่มประสิทธิภาพการเทรดและประหยัดเวลา แพลตฟอร์มนำเสนอชุดพื้นฐานทางการเงิน: stablecoin ค้ำประกันที่มีความหลากหลายซึ่งได้รับการสนับสนุนจากทรัพย์สิน cross-chain เช่น Bitcoin อนุพันธ์ trustless staking และการแลกเปลี่ยนแบบกระจายอำนาจเพื่อปลดปล่อยสภาพคล่องและนวัตกรรมทางการเงินที่มีอำนาจ Acala เป็นแพลตฟอร์มที่เข้ากันได้กับ Ethereum สำหรับแอปพลิเคชันทางการเงินเพื่อใช้ smart contract หรือโปรโตคอลในตัวพร้อมความสามารถ cross-chain ที่พร้อมใช้งานทันทีและการรักษาความปลอดภัยที่แข็งแกร่ง

[Discord](https://discord.gg/vdbFVCH) | [Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc)
