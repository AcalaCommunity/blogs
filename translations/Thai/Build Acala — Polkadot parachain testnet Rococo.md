# สร้าง Acala: Polkadot parachain testnet Rococo, ทำงานร่วมกับ Ren, Mandala testnet mania บน The Defiant | ส.ค. 2020

กรกฎาคมเป็นเดือนแห่งการสร้างร่วมกับผู้ทำงานร่วมกันในระบบนิเวศเช่น [Ren](https://renproject.io/) และ [Laminar](http://laminar.one/) ทดสอบเครือข่ายด้วยบัญชีและธุรกรรมใหม่หลายหมื่นรายการตลอดการทดสอบ Mandala Festival Season #3 แคมเปญและเตรียมพร้อมที่จะเปิดตัวบน Parachain testnet Rococo ของ Polkadot

![รูปสำหรับโพสต์](https://miro.medium.com/max/8000/1*6wJEyP0ojcA8zM3SZAPzqQ.jpeg)

# **อัพเดทการพัฒนา**

- **Polkadot's parachain testnet** [**Rococo:** เปิดตัว](https://polkadot.network/introducing-rococo-polkadots-parachain-testnet/)เมื่อต้นสัปดาห์นี้ ซึ่งเป็นก้าวสำคัญในการบูรณาการ cross-chain Parachains สามารถเชื่อมต่อกับ Relay chain เพื่อใช้การรักษาความปลอดภัยที่ใช้ร่วมกันได้ และยังสามารถส่งข้อความ cross-chain ที่คาดหวังไว้ได้ แม้ว่าจะจำกัดเฉพาะการส่งข้อความแนวนอนที่ Relay chain จะถูกใช้เพื่อกำหนดเส้นทางข้อความระหว่างสอง parachain Acala กำลังทำงานเพื่อลงทะเบียนกับ Rococo เพื่อทดสอบฟังก์ชันต่างๆ
- [**โมดูล RenVM สะพาน**](https://github.com/AcalaNetwork/Acala/tree/master/ecosystem-modules) **& การรวม renBTC:** ถูกปรับใช้บน Acala Mandala testnet TC4 ซึ่งเป็นก้าวแรกที่นำ renBTC มาสู่ Acala และระบบนิเวศ Polkadot ตอนนี้ renBTC เป็นโทเค็นค่าธรรมเนียม สามารถใช้เป็นหลักประกันสำหรับวงเงินเครดิต stablecoin และจดทะเบียนใน Acala DeX
- **Substrate RC4**: ตอนนี้ Mandala TC4 ได้รับการอัปเกรดเป็น [Substrate RC4](https://github.com/paritytech/substrate/releases/tag/v2.0.0-rc4) ซึ่งช่วยให้ทำธุรกรรมแบบอะตอมได้ ใกล้เคียงกับ smart contract ที่พร้อมสำหรับการผลิตเพียงก้าวเดียว และเร็วๆ นี้จะได้รับการอัปเกรดเป็น TC5 ล่าสุด เมื่อสรุปแคมเปญ testnet
- **Acala Pulse**: แดชบอร์ดการวิเคราะห์เพื่อติดตามสถิติของเครือข่ายอยู่ในระหว่างการปรับปรุงและจะเปิดตัวในสัปดาห์หน้า ผู้ใช้สามารถติดตามปัจจัยพื้นฐานของระบบ เช่น การออก aUSD ปริมาณ DeX และจำนวน DOT ในการ stake สภาพคล่อง เช่นเดียวกับความเสี่ยงของระบบ การชำระบัญชี และการประมูล เป็นต้น
- **การฝึกซ้อม Black Thursday & การปิดระบบฉุกเฉิน**: สัปดาห์หน้า [เป็นส่วนหนึ่งของเทศกาล Mandala](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#week-3-black-thursday-simulation) เราจะจำลองความผันผวนของ Black Thursday ทดสอบกลไกการชำระบัญชีแบบผสมที่เกี่ยวข้องกับ DeX และการประมูลเพื่อกู้คืนเงินกู้อย่างมีประสิทธิภาพ จากนั้นเราจะประกาศใช้ระบบ Emergency Shutdown ประมวลผลสินเชื่อคงค้างทั้งหมด และให้ผู้ใช้เรียกหลักประกันคืนจากตะกร้าสินทรัพย์ _เทศกาลสัปดาห์ที่ 3 กฎ & รางวัลอยู่ที่นี่_ [_ที่นี่_](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#week-3-black-thursday-simulation)_._

  ![รูปสำหรับโพสต์](https://miro.medium.com/max/2880/1*XQbgIIFPlzwrK8L1eXdKew.jpeg)

# **การอัพเดทระบบนิเวศ**

- [**Ren x Acala / Polkadot**](https://medium.com/acalanetwork/bringing-btc-to-polkadot-acala-x-ren-e7959855d5aa?source=collection_home---4------2-----------------------) **เพื่อ** นำ Bitcoin และสินทรัพย์ประเภทอื่น ๆ ที่แยกออกมาในอนาคตเข้าสู่ Acala และเข้าสู่จักรวาลมัลติเชนของ Polkadot ที่กว้างขึ้น
- [**Mandala Festival Season #3**](https://medium.com/acalanetwork/acala-mandala-festival-season-3-d0a6f155c154?source=collection_home---4------1-----------------------): เริ่มเมื่อสองสัปดาห์ก่อน สร้างความฮือฮาให้กับธุรกรรม **_100k+ รายการ บัญชีใหม่ 13k บัญชี $2.5+ ล้าน aUSD ที่ออกจากการค้ำประกัน renBTC และ 250+ (testnet) renBTC ที่ mint ตรวจสอบ [กิจกรรมบน Subscan](https://acala-testnet.subscan.io/)</li>
- [**Hackusama with Acala**](https://medium.com/acalanetwork/hackusama-ea1ddf3e945a): Acala เป็นพันธมิตรด้านการศึกษาของ Hackusama โดยให้บริการพาเลทรันไทม์ทั้งหมดและ[ไลบรารีทั่วไป](https://github.com/open-web3-stack/open-runtime-module-library) เช่น oracle และพาเลทหลายโทเค็น การสนับสนุนด้านเทคนิคและคำแนะนำแก่ ทีมสร้างโครงการ DeFi
- **Acala Foundation เป็นสมาชิกสภาแล้ว** เกี่ยวกับ Polkadot มีส่วนร่วมอย่างแข็งขันในการอภิปรายและการลงคะแนนเสียง Polkadot Direction ขอขอบคุณสำหรับการสนับสนุนอย่างต่อเนื่องของคุณ เพื่อให้เราสามารถเติบโต Polkadot และ DeFi ไปด้วยกัน 🚀 together</ul>

# **อัปเดตอีเวนท์**

- **รวม SF Blockchain Week**: Bette Chen ผู้ร่วมก่อตั้ง Acala พูดคุยเกี่ยวกับ DeFi  cross-chain ในการดำเนินการ ดู [รีเพลย์](https://next.brella.io/events/unitize2020/schedule/156155)
- **The Defiant**: Ruitao Su และ Bette Chen พูดคุยกับ Camila Russo บน Polkadot ว่าเป็นเลเยอร์ 0 ว่าระบบนิเวศมีการพัฒนาอย่างไรให้มี vertical เฉพาะของโดเมนและอีกมากมาย Podcast [ที่นี่](https://anchor.fm/camila-russo/episodes/Developers-Will-Wake-Up-to-the-Fact-That-Theres-a-Toolkit-to-Build-Full-Fledged-Customized-Chains-Acalas-Bette-Chen-eh7sp0/a-a2pmg6h) & อ่าน [เพิ่มเติม](https://twitter.com/DefiantNews/status/1287758518913765377?s=20)
- Bette Chen เป็น Outlierใน **Outlier Venture panel — “Prophesying the Future of Oracles”** ควบคู่ไปกับ MakerDAO, DIA, Set Protocol และ Aave ดูการสนทนาของ Bette เกี่ยวกับการ yield farming [ที่นี่](https://twitter.com/OVioHQ/status/1290644606892343297?s=20) & ดูแบบเต็มพาเนล [รีเพลย์](https://www.crowdcast.io/e/prophesying-oracles)

# เกี่ยวกับ Acala

[Acala](http://acala.network/) เป็นระบบการเงินแบบกระจายศูนย์แห่งแรกที่มีวิสัยทัศน์ในการสร้างความมั่นคงทางการเงิน สภาพคล่อง และการเข้าถึงกระแสหลัก **เครือข่าย Acala เป็นศูนย์กลางการเงินข้ามเครือข่ายสำหรับระบบนิเวศ Polkadot** และอื่นๆ แพลตฟอร์มนำเสนอชุดพื้นฐานทางการเงิน: stablecoin ค้ำประกันที่มีความหลากหลายซึ่งได้รับการสนับสนุนจากทรัพย์สิน cross-chain เช่น Bitcoin อนุพันธ์ trustless staking และการแลกเปลี่ยนแบบกระจายอำนาจเพื่อปลดปล่อยสภาพคล่องและนวัตกรรมทางการเงินที่มีอำนาจ เป็นแพลตฟอร์มเปิดแบบเปิดสำหรับ dApps ที่เน้นด้านการเงินเพื่อปรับใช้กับ smart contract หรือโปรโตคอลในตัวที่มีความสามารถ cross-chain ที่พร้อมใช้งานทันที ความปลอดภัย และการเพิ่มประสิทธิภาพทางการเงิน

# ร่วมกับเรา

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

หากต้องการติดตามความคืบหน้าในการเปิดตัว Acala โปรดสมัครรับจดหมายข่าว [จดหมายข่าวของ Acala](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc)

![รูปสำหรับโพสต์](https://miro.medium.com/max/1500/0*1KozUmtgLB7qV79q.jpeg)

Acala เป็นผู้รับทุนมูลนิธิ Web3 ที่น่าภาคภูมิใจ
