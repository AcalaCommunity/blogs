# แนวทางของ Karura ต่อการประมูล Crowdloan และ Parachain ที่จะเกิดขึ้นบน Kusama

## Karura เครือข่ายน้องสาวของ Acala และศูนย์กลาง DeFi ของ Kusama จะเริ่ม Crowdloan ในไม่ช้าเพื่อรับการสนับสนุนจากชุมชนสำหรับการประมูล Kusama Parachain ครั้งแรก

![Image for post](https://miro.medium.com/max/1600/0*1XypG_FOdz_or1ro)

Karura สร้างขึ้นในฐานะเครือข่ายน้องสาวของ Acala ด้วยโค้ดเดียวกัน เป็นเครือข่ายบล็อคเชนใหม่ที่ทุ่มเทเพื่อให้บริการชุมชน Kusama ในฐานะศูนย์กลางการเงินแบบกระจายอำนาจ (DeFi) หลัก ฮับ DeFi แบบข้ามสายของ Karura จะมอบเหรียญที่มีเสถียรภาพ (kUSD) สภาพคล่องสำหรับ KSM ที่เรียกว่า L-KSM, ความสามารถของ DEX, การยืม , การให้ยืม รวมถึงแอปพลิเคชันอื่นๆ

ไม่ว่า chain ใดๆ เช่น Karura ที่วางแผนที่จะเชื่อมต่อกับเครือข่ายมัลติเชน "เลเยอร์ศูนย์" ของ [Kusama](http://kusama.network) สำหรับความสามารถในการทำงานร่วมกันและการรักษาความปลอดภัยแบบ plug-and-play โดยเรียกว่าพาราเชน Kusama วางแผนที่จะมีสล็อต parachain มากกว่า 100 ช่องในอนาคต แต่เครือข่ายยังอยู่ในช่วงเริ่มต้น ดังนั้น เครือข่ายที่สร้างโดย Dr. Gavin Wood ผู้ก่อตั้ง Polkadot จึงเริ่มต้นด้วยช่อง parachain ที่มีอยู่อย่างจำกัด เพื่อเข้าถึงslot ของ Parachain ทีมที่มีความหวังต้องเข้าร่วมและชนะ [การประมูลเทียน](https://wiki.polkadot.network/docs/en/learn-auction) โดยใช้โทเค็น KSM ดั้งเดิมของ Kusama ซึ่งถูกล็อคไว้ในช่วงระยะเวลาการเช่าของ Parachain

Karura วางแผนที่จะเป็นเจ้าภาพ Crowdloan ครั้งแรกบน Kusama และเข้าร่วมในการประมูล Parachain รอบแรก ([รายละเอียดเกี่ยวกับการประมูล Parachain ที่นี่](https://wiki.polkadot.network/docs/en/learn-auction)) การประมูล Parachain สามารถเข้าถึงได้หลายวิธี และเราจะใช้เวลาสักครู่ด้านล่างเพื่ออธิบายแนวทางของ Karura ผู้ที่ต้องการเจาะลึกกระบวนการรับสล็อต parachain บน Kusama หรือ 'เครือข่ายลูกพี่ลูกน้อง' Polkadot ควรอ่าน [ภาพรวมโดยละเอียด](https://polkadot.network/obtaining-a-parachain-slot-on-polkadot/) ของบล็อก Polkadot

## **พื้นฐานของ Karura**

Karura เป็นเครือข่ายน้องสาวของ [Acala](http://acala.network) ที่มุ่งเน้นการนำ DeFi มาที่ Kusama เช่นเดียวกับ Acala กำลังนำ DeFi มาที่ Polkadot ที่มาของชื่อ Karura มาจากสิ่งมีชีวิตศักดิ์สิทธิ์ในภาษาญี่ปุ่น ที่มาจากเผ่าพันธุ์นกในศาสนาฮินดู ตามตำนานของญี่ปุ่น karura ได้รับการกล่าวขานว่าเป็นนกขนาดใหญ่ที่พ่นไฟได้ ซึ่งเข้ากันได้ดีกับความตั้งใจที่กล้าหาญและทรงพลังของเครือข่าย Karura ตัวแทนของแบรนด์ Karura คือนกฟีนิกซ์ นกที่ลุกเป็นไฟที่แสดงถึงความยืดหยุ่นผ่านการเกิดใหม่และการสร้างใหม่อย่างต่อเนื่อง

## **คุณสมบัติ DeFi และการปรับปรุงจาก Karura**

อนาคตจะถูกกำหนดโดยชุมชนโอเพ่นซอร์สของผู้สร้าง ปูทางสำหรับกรณีการใช้งานและแอปพลิเคชันใหม่ๆ บน Karura และ Acala Karura จะเริ่มต้นด้วยแอปพลิเคชั่นที่พร้อมใช้งานมากมาย และเนื่องจาก Karura เป็นแพลตฟอร์ม 'เลเยอร์ 1' นักพัฒนาจำนวนมากจึงปรับใช้แอพบนโครงสร้างพื้นฐานของ Karura ด้วย Karura จะเริ่มต้นชีวิตบน Kusama ด้วยแอพและกรณีการใช้งานที่ระบุไว้ในโพสต์บล็อกก่อนหน้านี้ด้านล่าง คุณยังสามารถ[**ลองใช้เลย**](https://apps.acala.network/)บน testnet ของ Karura และ Acala ที่เรียกว่า Mandala ตรวจสอบภาพรวมทั้งหมดเกี่ยวกับประโยชน์ของ Karura ที่มีต่อผู้ใช้ในบล็อกโพสต์ล่าสุด:

[ขอแนะนำ Karura: DeFi Parachain ของ Acala บน Kusama](https://medium.com/acalanetwork/introducing-karura-acalas-defi-parachain-on-kusama-af2f2695b07a)

# **แนวทางของ Karura ต่อการประมูล Crowdloan และ Parachain — ขอแนะนำ Paradrop**

Karura วางแผนที่จะเสนอราคาสำหรับสล็อต Parachain แรกบน Kusama และเป็นผู้บุกเบิกในกระบวนทัศน์ความปลอดภัยเครือข่ายที่รวบรวมผู้คนเข้ามาใหม่: **Crowdloan** และ **Paradrop** Karura จะดำเนินการรณรงค์การ trustless สำหรับชุมชน Kusama เพื่อล็อบบี้สำหรับการสนับสนุนจากผู้ถือ KSM Crowdloan เกี่ยวข้องกับผู้สนับสนุนเหล่านี้จะผูกมัด KSM ของพวกเขากับ Kusama เพื่อสนับสนุนการเสนอราคาของ Karura สำหรับการเช่า parachain ในการประมูล Kusama Parachain จรในที่สุดก็เริ่ม Paradrop

**KAR Paradrop**: เพื่อเป็นการตอบแทนสำหรับการสนับสนุนของผู้ถือ KSM KAR (โทเค็นดั้งเดิมของ Karura) จะแจกจ่ายให้กับผู้เข้าร่วมผ่าน Paradrop ในกรณีที่ Karura ประสบความสำเร็จในการประมูลและได้สัญญาเช่า Kusama parachain และการสร้างเครือข่ายของ Karura เกิดขึ้นที่ Kusama Karura จะนำ KAR ไปที่บัญชีที่ใช้ในการผูกมัด KSM เพื่อสนับสนุนการประมูล Parachain ของ Karura Paradrop จะมีผลตลอดระยะเวลาของสัญญาเช่าผ่านตารางการให้สิทธิ์ และจำนวน KAR ที่ผู้สนับสนุน Karura จะได้รับจะขึ้นอยู่กับระดับการสนับสนุนโดยผู้สนับสนุน Karura ซึ่งหมายความว่าผู้สนับสนุน Karura สามารถใช้ KAR ที่ได้รับเพื่อเข้าร่วมในการกำกับดูแลและการ staking ในระหว่างที่กำหนดตารางการให้สิทธิ์รับรู้

**ระยะเวลาพันธะ:** KSM จะถูกผูกมัดหรือ 'ถูกล็อค' ใน Kusama Relay Chain ในช่วงระยะเวลาการเช่าพาราเชนของ Karura ซึ่งหมายความว่าการสนับสนุน KSM ทั้งหมดถูกล็อกไว้ที่ Kusama เพื่อสนับสนุนการประมูล Parachain ของโครงการ การชนะการประมูลครั้งนี้ทำให้โปรเจ็กต์เข้าถึงการรักษาความปลอดภัย Proof of Stake แบบ Plug-and-play ของ Kusama ได้ แต่ KSM ทั้งหมด **ไม่สามารถเข้าถึงได้**สำหรับทีมโปรเจ็ค

KSM ใด ๆ ที่ผูกมัดกับ Kusama เพื่อสนับสนุนการประมูลการเช่า Parachain  ของ Karura จะถูกส่งคืนเต็มจำนวนเมื่อสิ้นสุดการเช่า parachain (ในกรณีที่การประมูลสำเร็จ) หรือคืนเมื่อสิ้นสุดการประมูล (หากการประมูลเป็น ไม่ประสบผลสำเร็จ) ซึ่งหมายความว่าทีมโปรเจ็คจะได้รับแรงจูงใจในการให้ความสำคัญกับการทำให้แน่ใจว่าโปรเจ็คและเครือข่ายที่เกี่ยวข้องมีการส่งมอบยูทิลิตี้ที่ตั้งใจไว้และมีการใช้งานจริงในแง่ของผู้ใช้และธุรกรรม

ผู้เข้าร่วมชุมชน Kusama จะมีตัวเลือกในการล็อคโทเค็นของพวกเขาบน Kusama เป็นระยะเวลาหนึ่ง (6, 12 หรือ 24 เดือน TBD) ทีมงาน Karura จะพิจารณาความชอบของชุมชน Kusama เมื่อตัดสินใจเกี่ยวกับระยะเวลาของสัญญาเช่า parachain ที่จะเสนอราคา **เตรียมพบกับแบบฟอร์มลงทะเบียนในอีกไม่กี่วันข้างหน้า โดยเราจะเริ่มประเมินความชอบของชุมชนในการตัดสินใจเหล่านี้**

**จำนวน KAR Paradrop ไม่สามารถคาดเดาได้:** ระดับการสนับสนุนที่แน่นอนที่ Karura จะต้องปรากฏเป็นผู้ชนะการประมูลท่ามกลางผู้เสนอราคาที่แข่งขันกันอื่นๆ ไม่เป็นที่รู้จัก และระยะเวลาของการเช่า parachain ที่ Karura จะเสนอราคานั้นยังไม่เป็นที่แน่ชัดในปัจจุบัน . With this said, the exact amount of KAR that will be subject to Paradrop to Karura supporters in recognition of their support for the upcoming Crowdloan will be unknown till the end of the auction. However, Karura will soon provide estimates for your reference. In a completely hypothetical example, a Karura supporter bonding X amount of KSM for Karura’s successful bid for a 6-months parachain lease would be recognized by a Paradrop of 5 KAR for her support; the same amount of KSM bonded in support of a successful bid for a 12-month parachain lease would be recognised with a Paradrop of 10 KAR given the extended duration of support.

**An _Actual_ ‘Fair’ Launch:** KAR will be Paradropped to Karura supporters in recognition of their support for Karura’s Crowdloan upon Karura network genesis on Kusama, but will be unlocked over time for transfer throughout the parachain lease period. However the full amount of the KAR Paradrop can be used for governance and other non-transfer functions to allow participation by Karura supporters in such functions from the outset of Paradrop to encourage participation and building of a strong and well-intentioned community from the ground up.

## **Next Steps and Getting Involved**

The Karura Crowdload and auction are rapidly approaching. We will soon be launching the Karura Crowdloan website, the Crowdloan registration and preferences-gathering process, and rolling out more details as they come.

The best way to stay in the loop is to join the [**Acala/Karura Discord**](https://discord.gg/HpsZx5r)**,** follow [**Karura on Twitter**](https://twitter.com/KaruraNetwork)**,** and follow [**Acala on Twitter**](https://twitter.com/AcalaNetwork).

# **เกี่ยวกับ Karura**

Karura is the decentralized financial hub of Kusama. The network is built as Acala’s sister network with nearly the same codebase — the two platforms enable a scalable, user-friendly, and fast cross-chain DeFi ecosystem for Kusama and Polkadot. Karura’s parachain is a fast-moving and powerful platform that enables efficient, inexpensive, and sophisticated financial applications, improving trading effectiveness and saving time. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Kusama and Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations.
