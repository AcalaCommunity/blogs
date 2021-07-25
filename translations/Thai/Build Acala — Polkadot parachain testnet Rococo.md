# สร้าง Acala: Polkadot parachain testnet Rococo, ทำงานร่วมกับ Ren, Mandala testnet mania บน The Defiant | ส.ค. 2020

กรกฎาคมเป็นเดือนแห่งการสร้างร่วมกับผู้ทำงานร่วมกันในระบบนิเวศเช่น [Ren](https://renproject.io/) และ [Laminar](http://laminar.one/) ทดสอบเครือข่ายด้วยบัญชีและธุรกรรมใหม่หลายหมื่นรายการตลอดการทดสอบ Mandala Festival Season #3 แคมเปญและเตรียมพร้อมที่จะเปิดตัวบน Parachain testnet Rococo ของ Polkadot

![Image for post](https://miro.medium.com/max/8000/1*6wJEyP0ojcA8zM3SZAPzqQ.jpeg)

# **อัพเดทการพัฒนา**

- **Polkadot's parachain testnet** [**Rococo:** เปิดตัว](https://polkadot.network/introducing-rococo-polkadots-parachain-testnet/)เมื่อต้นสัปดาห์นี้ ซึ่งเป็นก้าวสำคัญในการบูรณาการ cross-chain Parachains สามารถเชื่อมต่อกับ Relay chain เพื่อใช้การรักษาความปลอดภัยที่ใช้ร่วมกันได้ และยังสามารถส่งข้อความ cross-chain ที่คาดหวังไว้ได้ แม้ว่าจะจำกัดเฉพาะการส่งข้อความแนวนอนที่ Relay chain จะถูกใช้เพื่อกำหนดเส้นทางข้อความระหว่างสอง parachain Acala กำลังทำงานเพื่อลงทะเบียนกับ Rococo เพื่อทดสอบฟังก์ชันต่างๆ
- [**โมดูล RenVM สะพาน**](https://github.com/AcalaNetwork/Acala/tree/master/ecosystem-modules) **& การรวม renBTC:** ถูกปรับใช้บน Acala Mandala testnet TC4 ซึ่งเป็นก้าวแรกที่นำ renBTC มาสู่ Acala และระบบนิเวศ Polkadot ตอนนี้ renBTC เป็นโทเค็นค่าธรรมเนียม สามารถใช้เป็นหลักประกันสำหรับวงเงินเครดิต stablecoin และจดทะเบียนใน Acala DeX
- **Substrate RC4**: ตอนนี้ Mandala TC4 ได้รับการอัปเกรดเป็น [Substrate RC4](https://github.com/paritytech/substrate/releases/tag/v2.0.0-rc4) ซึ่งช่วยให้ทำธุรกรรมแบบอะตอมได้ ใกล้เคียงกับ smart contract ที่พร้อมสำหรับการผลิตเพียงก้าวเดียว และเร็วๆ นี้จะได้รับการอัปเกรดเป็น TC5 ล่าสุด เมื่อสรุปแคมเปญ testnet
- **Acala Pulse**: แดชบอร์ดการวิเคราะห์เพื่อติดตามสถิติของเครือข่ายอยู่ในระหว่างการปรับปรุงและจะเปิดตัวในสัปดาห์หน้า ผู้ใช้สามารถติดตามปัจจัยพื้นฐานของระบบ เช่น การออก aUSD ปริมาณ DeX และจำนวน DOT ในการ stake สภาพคล่อง เช่นเดียวกับความเสี่ยงของระบบ การชำระบัญชี และการประมูล เป็นต้น
- **การฝึกซ้อม Black Thursday & การปิดระบบฉุกเฉิน**: สัปดาห์หน้า [เป็นส่วนหนึ่งของเทศกาล Mandala](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#week-3-black-thursday-simulation) เราจะจำลองความผันผวนของ Black Thursday ทดสอบกลไกการชำระบัญชีแบบผสมที่เกี่ยวข้องกับ DeX และการประมูลเพื่อกู้คืนเงินกู้อย่างมีประสิทธิภาพ จากนั้นเราจะประกาศใช้ระบบ Emergency Shutdown ประมวลผลสินเชื่อคงค้างทั้งหมด และให้ผู้ใช้เรียกหลักประกันคืนจากตะกร้าสินทรัพย์ _เทศกาลสัปดาห์ที่ 3 กฎ & รางวัลอยู่ที่นี่_ [_ที่นี่_](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#week-3-black-thursday-simulation)_._

  ![Image for post](https://miro.medium.com/max/2880/1*XQbgIIFPlzwrK8L1eXdKew.jpeg)

# **การอัพเดทระบบนิเวศ**

- [**Ren x Acala / Polkadot**](https://medium.com/acalanetwork/bringing-btc-to-polkadot-acala-x-ren-e7959855d5aa?source=collection_home---4------2-----------------------) **เพื่อ** นำ Bitcoin และสินทรัพย์ประเภทอื่น ๆ ที่แยกออกมาในอนาคตเข้าสู่ Acala และเข้าสู่จักรวาลมัลติเชนของ Polkadot ที่กว้างขึ้น
- [**Mandala Festival Season #3**](https://medium.com/acalanetwork/acala-mandala-festival-season-3-d0a6f155c154?source=collection_home---4------1-----------------------): เริ่มเมื่อสองสัปดาห์ก่อน สร้างความฮือฮาให้กับธุรกรรม **_100k+ รายการ บัญชีใหม่ 13k บัญชี $2.5+ ล้าน aUSD ที่ออกจากการค้ำประกัน renBTC และ 250+ (testnet) renBTC ที่ mint ตรวจสอบ [กิจกรรมบน Subscan](https://acala-testnet.subscan.io/)</li>
- [**Hackusama with Acala**](https://medium.com/acalanetwork/hackusama-ea1ddf3e945a): Acala is an education partner for Hackusama, providing all of its runtime pallets and [common libraries](https://github.com/open-web3-stack/open-runtime-module-library) such as oracle and multi-token pallet, technical support and advice to the teams building DeFi projects.
- **Acala Foundation is now a council member** on Polkadot actively participating in Polkadot Direction riot discussion and voting. We appreciate your continued support so we can grow Polkadot and DeFi together 🚀</ul>

# **Events Update**

- **Unitize SF Blockchain Week**: Bette Chen co-founder of Acala talked about cross-chain DeFi in action. Watch [replay](https://next.brella.io/events/unitize2020/schedule/156155).
- **The Defiant**: Ruitao Su and Bette Chen chatted with Camila Russo on Polkadot being layer 0, how the ecosystem is evolving to have many domain-specific chain verticals and more. Podcast [here](https://anchor.fm/camila-russo/episodes/Developers-Will-Wake-Up-to-the-Fact-That-Theres-a-Toolkit-to-Build-Full-Fledged-Customized-Chains-Acalas-Bette-Chen-eh7sp0/a-a2pmg6h) & read [more](https://twitter.com/DefiantNews/status/1287758518913765377?s=20).
- Bette Chen being the outlier on the **Outlier Venture panel — “Prophesying the Future of Oracles”** alongside MakerDAO, DIA, Set Protocol and Aave. See Bette chat about yield farming [here](https://twitter.com/OVioHQ/status/1290644606892343297?s=20) & watch the full panel [replay](https://www.crowdcast.io/e/prophesying-oracles).

# About Acala

[Acala](http://acala.network/) is a first-of-its-kind decentralized finance consortium with a vision to bring financial stability, liquidity and accessibility to the mainstream. **The Acala Network is a cross-chain finance hub for the Polkadot ecosystem** and beyond. It offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative and a decentralized exchange to unleash liquidity and power financial innovations. It is the go-to open platform for finance-oriented dApps to deploy to using smart contracts or built-in protocols with out-of-box cross-chain capabilities, security and financial optimizations.

# Join Us

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala launch, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

![Image for post](https://miro.medium.com/max/1500/0*1KozUmtgLB7qV79q.jpeg)

Acala is a proud Web3 Foundation Grantee
