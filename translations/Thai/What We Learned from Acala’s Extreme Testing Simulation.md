# สิ่งที่เราเรียนรู้จากการจำลองการทดสอบสุดขั้วของ Acala

## แคมเปญ testnet 3 สัปดาห์ของ Acala ได้สิ้นสุดลงแล้ว โดยเน้นถึงความสำคัญของ Canary Network และนำไปสู่การปรับปรุงทางเทคนิคหลายประการสำหรับ network

![Image for post](https://miro.medium.com/max/1600/1*lGVbzGOgp5M3DqCPtAds8A.jpeg)

โดย: [Bette Chen](https://medium.com/u/8d475d21e811?source=post_page-----5ef5769a0902--------------------------------)

Acala [Mandala Fest Season #3](https://medium.com/acalanetwork/acala-mandala-festival-season-3-d0a6f155c154) ซึ่งเป็นแคมเปญ testnet 3 สัปดาห์ ได้ข้อสรุปเรียบร้อยแล้วในวันที่ 17 สิงหาคม เป็นวิธีที่ยอดเยี่ยมสำหรับเราในการสาธิตความคืบหน้าการพัฒนาของเราต่อชุมชนโดยการทดสอบระบบและโปรโตคอลภายใต้ภาระหนักและสถานการณ์ที่รุนแรงในโดยมีการให้รางวัลแก่ผู้เข้าร่วม

เราได้รับการสนับสนุน ความกระตือรือร้นที่จะมีส่วนร่วมจากชุมชนอย่างท่วมท้น นี่คือสถิติบางส่วนที่เราได้เห็น:

✅ 14,500 + บัญชีใหม่

⛓️ 140,000 + ธุรกรรมที่มีความหมาย

💰 $52 million มูลค่ารวมที่ถูกล็อค

💲 $25 million aUSD ที่ใช้งาน

**ไฮไลท์ของวัลมีดังต่อไปนี้ และผลลัพธ์ทั้งหมด** [**ที่นี่**](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#season-3-prize-giving)**.**

😎 สัปดาห์ที่ 1 รางวัลสำหรับผู้ใช้ 2,105 คน จากทั้งหมด 10,525 คนที่มีคุณสมบัติ

[⌛](https://emojipedia.org/hourglass-done/) รางวัลสัปดาห์ที่ 2 ตกเป็นของเทรดเดอร์ 10 อันดับแรกด้วยผลตอบแทนเฉลี่ย 24,200%

🌋 รางวัลสัปดาห์ที่ 3 ให้แก่ผู้ใช้งาน 200 คน

✍️ 10 รางวัลสำหรับ bloggers/vloggers

🐞 45 รางวัลสำหรับนักล่าบัค

🤖️ รางวัลการล่าโค้ด 1 รางวัล

เรายังได้เรียนรู้บทเรียนอันล้ำค่าบางอย่าง ซึ่งบางบทเรียนก็ยืนยันความคิดของเราอีกครั้ง ในขณะที่บางบทเรียนได้นำไปสู่การปรับปรุง

# ความสำคัญของ Canary Network

การพัฒนาบล็อกเชนแบบดั้งเดิมประกอบด้วย testnet และสภาพแวดล้อมการผลิตเต็มรูปแบบเท่านั้น อย่างไรก็ตาม เราเชื่อว่าบล็อกเชนไม่สามารถทดสอบได้อย่างเหมาะสมหากไม่มีเงื่อนไขทางเศรษฐกิจที่แท้จริง จากแคมเปญ Mandala testnet เห็นได้ชัดว่ามีรางวัลประปราย (ส่วนใหญ่ผ่านการจับรางวัลสำหรับผู้เข้าร่วม) ในขณะที่สามารถทดสอบฟังก์ชันการทำงานและความสามารถในการใช้งานได้จนถึงส่วนขยายขนาดใหญ่ พลวัตทางเศรษฐกิจ ประสิทธิภาพของสภาพคล่อง และความเสี่ยงที่ไม่สามารถสำรวจได้อย่างเต็มที่ใน testnet ที่ไม่มีค่าเช่น Mandala

เช่นเดียวกับเครือข่าย Canary ของ Polkadot [Kusama](http://kusama.network) Acala ได้ติดตั้งเครือข่าย Canary [Karura](https://github.com/AcalaNetwork/Acala/wiki/1.-Get-Started#acala-trilogy-networks) ทั้งสองเครือข่ายมีมูลค่าทางเศรษฐกิจที่แท้จริง แต่ต่ำกว่าเครือข่ายหลัก (Acala ในกรณีของเรา) Karura Network มีมูลค่าทางเศรษฐกิจซึ่งแสดงเป็นโทเค็นเครือข่ายต้นแบบ [KAR](https://github.com/AcalaNetwork/Acala/wiki/V.-ACA-&-KAR) จะเปิดตัวเป็น Parachain บนเครือข่าย Kusuma และให้พื้นฐานทางการเงินแก่ระบบนิเวศของ Kusama เช่น การยอมรับ KSM เป็นหลักประกันสำหรับวงเงินเครดิตของ Stablecoin

# บทเรียนจากการจำลอง Black Thursday — สภาพคล่องคือราชา

ตอนนี้เราอาจได้ตระหนักว่าการยอมรับความเสี่ยงทางการเงินของระบบการเงินแบบกระจายอำนาจ (บนบล็อคเชน) นั้นถูกกำหนดโดยความสามารถและข้อจำกัดทางเทคนิคของบัญชีแยกประเภท เราได้สรุปปัญหาพื้นฐานที่นำไปสู่เหตุการณ์ Black Thursday วันที่ 12 มีนาคมของ MakerDAO [ที่นี่](https://medium.com/acalanetwork/regaining-confidence-in-decentralized-stablecoins-bd98ba8e3c83):

- ประสิทธิภาพมีคอขวดของเครือข่ายพื้นฐาน
- ความไร้ประสิทธิภาพในการชำระบัญชีสินเชื่อที่มีหลักประกันความเสี่ยงหรือ CDPs
- ความไร้ประสิทธิภาพของผู้คุม & วิกฤติสภาพคล่อง

## เราได้ดำเนินการปรับปรุงดังต่อไปนี้:

- **คุณภาพของบริการสำหรับการดำเนินงานของ oracle:** ธุรกรรมของ oracle ได้รับการจัดลำดับความสำคัญและรวมอยู่ในบล็อกเสมอ ดังนั้นฟีดราคาจึงเป็นข้อมูลล่าสุดและไม่ได้รับผลกระทบจากการรับส่งข้อมูลในเครือข่าย
- **ตัวจัดการสภาพคล่องอัตโนมัติ** โดยใช้ [Off-chain Workers](https://www.parity.io/substrate-off-chain-workers-secure-and-efficient-computing-intensive-tasks/): ผู้ดำเนินการภายนอกเช่น Keepers จำเป็นในโปรโตคอลเช่น Maker เท่านั้น เนื่องจาก Ethereum หรือเทคโนโลยีที่คล้ายกันไม่สามารถให้ตัวจัดกำหนดการอัตโนมัติที่ปลอดภัยบนโหนดของบล็อกเชน Acala ใช้เครื่องชำระบัญชีอัตโนมัติที่สามารถประเมินตำแหน่งสินเชื่ออย่างมีประสิทธิภาพในทุกช่วงตึก
- **Hybrid liquidation mechanism with DEX and auction:** the system will automatically liquidate collaterals on the DEX if price and slippage are favorable, to avoid price inefficiencies on auctions.
- **High throughput and specialization:** Acala has unoptimized throughput of 1000 tps; in Polkadot’s multi-chain universe, each shard/parachain is likely to be optimized for its use case. For example, Acala will be the financial shard optimized for DeFi operations, while another chain might specialize in gaming or breeding cats. The real throughput of Polkadot would be 1000 tps multiplied by the total number of shards/parachains connected.

During the campaign, Acala ran a Black Thursday drill to simulate severe price volatility resulting in liquidation of risky loan positions, followed by a system Emergency Shutdown. While under heavy load, the system performed as expected, and eventually all loans were processed and collaterals were returned to users.

📉 14,400+ loans were liquidated

⚡️ $1.37 million of assets were liquidated

# The Power of Cross-chain Liquidity

Acala is the finance hub of Polkadot’s multi-chain universe. It provides a suite of financial primitives including a multi-collateralized stablecoin, trustless staking derivative, and a decentralized exchange. These primitives are offered via Acala’s DApp directly to the end-users and also as SDKs for more DApps to be built upon. We see a more interconnected, autonomous, sophisticated, cross-blockchain finance ecosystem on the cusp of emergence.

We have integrated with Ren and Laminar and showcased the power of cross-chain liquidity:

₿ 1,403 renBTC was minted

👨‍🌾 $1.4 million worth of renBTC traded on DeX, $5.5 million used in lending

🌈 $4.3 million aUSD crossed to Laminar for synthetic asset (forex, gold, synthetic BTC & ETH) margin trading

Learn more about Acala cross-chain DeFi use cases [here](https://github.com/AcalaNetwork/Acala/wiki/T.-Cross-chain-DeFi); come and create the next killer DeFi project using our framework, DeFi primitives and SDKs. Our offerings are production-grade and production-ready. We were also an educational partner in Kusama’s recent Hackusama event, and you can learn more about building with Acala [here](https://medium.com/acalanetwork/hackusama-ea1ddf3e945a).

# Join Us

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launch, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).
