# การสร้าง Acala — กันยายน 2020 | Testnet Parachain ของ Acala รอบการระดมทุนใหม่ smart contract และความเข้ากันได้ของ Ethereum

![รูปสำหรับโพสต์](https://miro.medium.com/max/1600/0*rPcIWxu2NiMMUEpU)

ถึงเวลาสำหรับ **Building Acala** เวอร์ชันเดือนกันยายน 2020 และหากคุณเพิ่งเริ่มใช้ Acala เรายินดีต้อนรับ! [Acala](http://acala.network) เป็นศูนย์กลางทางการเงินแบบกระจายอำนาจของ Polkadot ที่ทำให้ใช้งานหรือสร้างแอปพลิเคชันทางการเงินได้อย่างรวดเร็วและง่ายดาย เพิ่มประสิทธิภาพการเทรดและประหยัดเวลา เมื่อมองย้อนกลับไปในเดือนสิงหาคม เป็นเดือนที่เน้นย้ำด้วยเหตุการณ์สำคัญที่ Acala Parachain เริ่มทำงานและถ่ายโอนโทเค็นได้สำเร็จบน Polkadot testnet นักลงทุนรอบใหม่ พันธมิตรเชิงกลยุทธ์ การเปิดตัว smart contract และความเข้ากันได้ของ Ethereum บน Acala อ่านต่อด้านล่างสำหรับเหตุการณ์ทั้งหมดเกี่ยวกับระบบนิเวศ Acala และหลังจากนั้น เราขอเชิญคุณมาร่วมกับเราทาง [Twitter](https://twitter.com/acalanetwork) และ [Telegram](https://t.me/AcalaOfficial)

# **อัพเดทการพัฒนา**

- **Acala เปิดตัว Smart Contracts และความเข้ากันได้ของ Ethereum สำหรับ Polkadot DeFi** [**(Medium)**](https://medium.com/acalanetwork/acala-unveils-smart-contracts-and-ethereum-compatibility-for-polkadot-defi-588b3891e53d)**:** Acala รองรับ EVM และ ink แล้ว! พาเลทบน Substrate เปิดใช้งาน Smart Contracts แบบ Solidity และ Wasm สำหรับนักพัฒนา

- **Acala เปิดตัว Parachain ตัวแรกบน Polkadot Testnet** [(**Medium**)](https://medium.com/acalanetwork/acala-launches-the-1st-parachain-on-polkadot-testnet-682c02bad08b): Acala ได้เปิดตัว Parachain บน testnet ของ Polkadot เพื่อเตรียมพร้อมสำหรับการปรับใช้ mainnet บน Kusama และ Polkadot

- **การถ่ายโอนและแลกเปลี่ยนโทเค็น cross-chain ที่ประสบความสำเร็จครั้งแรกใน Acala DEX** [(**Twitter**)](https://twitter.com/AcalaNetwork/status/1297851737525481473?s=20): Acala ได้เปิดใช้งานชุด DeFi เต็มรูปแบบบน testnet parachain: ทดสอบว่า DOT สามารถโอนไปยัง Acala Parachain ได้อย่างน่าเชื่อถือ ใช้เป็นโทเค็นค่าธรรมเนียมพื้นฐาน และใช้เพื่อเข้าร่วมใน DeFi เช่น ใช้ DeX เพื่อแลกเปลี่ยนหรือค้ำประกันเครดิต USD

- **การโอน Stablecoin cross-chain ที่ประสบความสำเร็จครั้งแรกจาก Acala ไปยัง Laminar บน testnet** [(**Twitter**)](https://twitter.com/bettechentt/status/1298768242333237248?s=20): Acala ได้รับการรวมเข้ากับ [Laminar](https://www.laminar.one/) 2> parachain testnet สำหรับการถ่ายโอนโทเค็น cross-chain และการใช้ฟังก์ชัน DeFi ตัวอย่างวิดิโอ:

- **Acala สร้างและเปิดตัวพาเลท _xtoken_ สำหรับการโอนโทเค็นในระบบนิเวศ Polkadot** [(**Github**)](https://github.com/open-web3-stack/open-runtime-module-library/tree/rococo/xtokens): Parachain ใด ๆ ที่ใช้ พาเลท xtoken ที่สร้างโดย Acala สามารถรวมเข้ากับ Acala สำหรับการโอนโทเค็นได้แล้ว Xtoken ได้รับการเผยแพร่เป็น library ที่ดีสำหรับ Parachain ใด ๆ ที่จะใช้

- **Acala สร้างและเผยแพร่โค้ดเพื่อช่วยให้เชนที่อยู่บน Substrate กลายเป็น Parachain บน Polkadot หรือ Kusama** [(**Github**)](https://github.com/AcalaNetwork/Acala/pull/362): ลองดู PR ด้านบนนี้ พร้อมกับความพยายามในการ refactoring อย่างต่อเนื่อง ([**Github**](https://github.com/AcalaNetwork/Acala/compare/rococo-rc6)) เพื่อสนับสนุน chains ที่ทำงานเป็น Substrate chains หรือ parachains ที่เป็นอิสระ

**การอัปเดตการพัฒนาอื่น ๆ ที่จะเกิดขึ้น:**

- การเปิดตัว testnet ครั้งต่อไปของ Acala จะเปิดใช้งานความสามารถในการทำ smart contract บน Acala พร้อมแนวทางปฏิบัติเกี่ยวกับขั้นตอนความพร้อมในการผลิต
- รับชมการผสานการทำงานแบบ cross-parachain และ cross-blockchain เพิ่มเติมได้ในเร็วๆ นี้

# **การอัพเดทระบบนิเวศ**

- **Acala เพิ่ม Series A เพิ่มเติมสำหรับ Polkadot DeFi Hub ก่อนการเปิดตัว Parachain ที่จะเกิดขึ้น (**[**Medium**](https://medium.com/acalanetwork/acala-raises-additional-series-a-for-polkadot-defi-hub-ahead-of-upcoming-parachain-launch-22fdee9c2be9)**)**: Acala ได้ระดมเงินทุนเพิ่มเติมพร้อมกับ พาร์ทเนอร์ทางธุรกิจสำหรับความเชี่ยวชาญด้าน DeFi การจัดหาสภาพคล่อง และการจัดการความเสี่ยง ([Twitter](https://twitter.com/bettechentt/status/1299497896207773696?s=20))
- **สิ่งที่เราเรียนรู้จากการจำลองการทดสอบขั้นสูงสุดของ Acala** ([Medium](https://medium.com/acalanetwork/what-we-learned-from-acalas-extreme-testing-simulation-5ef5769a0902)): แคมเปญเครือข่ายทดสอบ 3 สัปดาห์ของ Acala ได้สิ้นสุดลงแล้ว โดยเน้นย้ำถึงความสำคัญของ Canary Network และนำไปสู่การปรับปรุงทางเทคนิคหลายประการสำหรับ เครือข่าย

สถิติบางส่วนที่เราเห็นระหว่างแคมเปญ community testnet นี้:

✅ 14,500 + บัญชีใหม่ | ⛓️ 140,000 + ธุรกรรมที่มีความหมาย | 💰มูลค่ารวมที่ถูกล็อค $52 ล้าน | 💲 aUSD 25 ล้านเหรียญสหรัฐที่ถูกใช้งาน

ไฮไลท์ของรางวัลมีดังต่อไปนี้ และผลการแข่งขันฉบับเต็มเผยแพร่บน [Github](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#season-3-prize-giving):

😎 สัปดาห์ที่ 1 รางวัลสำหรับผู้ใช้ 2,105 คน จากทั้งหมด 10,525 คนที่มีคุณสมบัติ

⌛ รางวัลสัปดาห์ที่ 2 ตกเป็นของเทรดเดอร์ 10 อันดับแรกด้วยผลตอบแทนเฉลี่ย 24,200%

🌋 รางวัลสัปดาห์ที่ 3 ให้แก่ผู้ใช้งาน 200 คน

✍️ 10 รางวัลสำหรับ bloggers/vloggers

🐞 45 รางวัลสำหรับนักล่าบัค

🤖️ รางวัลการล่าโค้ด 1 รางวัล

# **Acala ในสื่อ**

![รูปสำหรับโพสต์](https://miro.medium.com/max/2576/1*v2Ndsw3UwNTj0EhQNbFykw.png)

[CoinDesk](https://www.coindesk.com/acala-polkadot-defi-7m-pantera-saft)

![รูปสำหรับโพสต์](https://miro.medium.com/max/2562/1*z4iztwspAQT0KgfGt4jp_w.png)

[Yahoo Finance](https://finance.yahoo.com/news/polkadot-based-defi-project-acala-092543143.html)

![รูปสำหรับโพสต์](https://miro.medium.com/max/2274/1*ZA2JHJmNc15TXwClrwE_GQ.png)

[CryptoBriefing](https://cryptobriefing.com/acala-network-polkadots-makerdao-comes-ethereum/)

# **กิจกรรม**

- [Acala เข้าร่วม Cross-chain DeFi AMA กับ Acala, Laminar & Ren สำหรับ 650+ คน](https://twitter.com/AcalaNetwork/status/1295477682214338560?s=20)
- 16–18 ก.ย. : Acala จะพูดที่งาน China International Blockchain Business Future Development Summit ครั้งที่ 3 โดย Chain News และ inkrpto
- Ruitao ผู้ร่วมก่อตั้ง Acala ผู้ตัดสิน Kusama Hackathon, Hackusama และ ผู้สนับสนุน Acala ที่ได้รับการสนับสนุนในฐานะหุ้นส่วนด้านเทคโนโลยีและการศึกษา ([Hackusama with Acala](https://medium.com/acalanetwork/hackusama-ea1ddf3e945a)) แม้ว่า Hackathon นี้จะจบลง แต่การสร้างยังคงดำเนินต่อไป! เรากำลังมองหาทีมงานที่ยอดเยี่ยมในการสร้างผลิตภัณฑ์หรือระบบการเงินที่เกี่ยวข้องกับ DeFi มาสร้างด้วยกันกับ Acala ([Github — สร้างด้วย Acala](https://github.com/AcalaNetwork/Acala/wiki/U.-Build-with-Acala))

![รูปสำหรับโพสต์](https://miro.medium.com/max/1358/0*qMAanMu2kGLUXByX)

# ร่วมกับเรา

[Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

หากต้องการติดตามความคืบหน้าเกี่ยวกับการเปิดตัว Acala Parachain บน Polkadot และ Kusama โปรดสมัครรับข้อมูล [จดหมายข่าวของ Acala](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc)

# **เกี่ยวกับ Acala**

[Acala](http://acala.network/) เป็นศูนย์กลางทางการเงินแบบกระจายอำนาจของ Polkadot ที่ทำให้ใช้งานหรือสร้างแอปพลิเคชันทางการเงินได้อย่างรวดเร็วและง่ายดาย เพิ่มประสิทธิภาพการเทรดและประหยัดเวลา แพลตฟอร์มนำเสนอชุดพื้นฐานทางการเงิน: stablecoin ค้ำประกันที่มีความหลากหลายซึ่งได้รับการสนับสนุนจากทรัพย์สิน cross-chain เช่น Bitcoin อนุพันธ์ trustless staking และการแลกเปลี่ยนแบบกระจายอำนาจเพื่อปลดปล่อยสภาพคล่องและนวัตกรรมทางการเงินที่มีอำนาจ Acala เป็นแพลตฟอร์มเปิดตามความจริง(de facto) สำหรับแอปพลิเคชันด้านการเงินเพื่อใช้ smart contract หรือโปรโตคอลในตัวที่มีความสามารถ cross-chain, ความปลอดภัย และการเพิ่มประสิทธิภาพทางการเงิน
