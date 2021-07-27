# ประกาศ Acala Mandala Testnet, พาร์ทเนอร์ที่แข็งแกร่ง และโครงการระบบนิเวศ

เรารู้สึกตื่นเต้นที่ได้เปิดตัวเครือข่ายสามอันแรกสำหรับ Acala — Mandala Test Network, ประกาศเกี่ยวกับพันธมิตรของเรา และ Acala Ecosystem Program

![Image for post](https://miro.medium.com/max/5000/0*9hFZBkxybL4cD0nm.jpg)

# การเปิดเผย 3เครือข่ายของ Acala

[เครือข่าย Acala](https://medium.com/acalanetwork/acala-powering-cross-blockchain-open-finance-applications-on-polkadot-abb6075a6edf) จะเพิ่มพลังให้กับเหรียญ stablecoin ที่มีหลายหลักประกันและกระจายอำนาจแบบ cross-chain และทำหน้าที่เป็นหน่วยการสร้างบล็อค DeFi สำหรับระบบนิเวศ Polkadot วิวัฒนาการของเครือข่าย Acala จะถูกมาร์คโดย 3 เครือข่ายนี้:

- **Mandala Test Network**: เป็นสนามเด็กเล่นที่ปราศจากความเสี่ยงและไม่มีมูลค่าของเรา ผู้ใช้ และนักพัฒนาเพื่อทดสอบการทำงานของ Acala คาดว่าจะมีบั๊ค ความวุ่นวาย และการรีบูตโดยไม่ได้แจ้งให้ทราบล่วงหน้า
- **เครือข่าย Karura**: เป็นรุ่นทดลองของ Acala ที่ยังไม่ได้ตรวจสอบและทดลอง ซึ่งจะเข้าร่วมเครือข่าย Kusama ในฐานะ parachain มันจะมีมูลค่าทางเศรษฐกิจที่แสดงเป็นโทเค็นดั้งเดิมของ KAR และ KSM สามารถใช้เป็นหลักประกันสำหรับ kaUSD
- **Acala Mainnet**: จะเชื่อมต่อกับเครือข่าย Polkadot เมื่อเปิดตัว

# Mandala Network

คาดว่าจะมีข้อบกพร่องและการรีบูตโดยไม่ได้แจ้งให้ทราบล่วงหน้า

Mandala เป็นเครือข่ายทดสอบสำหรับ Acala อนุญาตให้ผู้ใช้ ทีม และนักพัฒนาสามารถทดสอบการทำงานของฟังก์ชั่น Stablecoin ได้สัมผัสกับการกำกับดูแลของ Acala และสร้างการบูรณาการในสภาพแวดล้อมที่ปราศจากความเสี่ยง

# ทำไมถึง Mandala?

ทำไม Acala ถึงเป็นที่หนึ่ง? Acala เป็นเทพผู้ไม่เคลื่อนไหวและผู้พิทักษ์ประตูในพระพุทธศาสนา ในเชิงสัญลักษณ์ stablecoin เป็นรากฐานของผู้พิทักษ์การเงินแบบกระจายอำนาจ **Mandala ตั้งใจจะเป็นประตูสู่ทั้งสองเครือข่ายของ Acala ต่อจากนี้** ที่ซึ่งเราจะได้ลิ้มรสของ Acala, ลองทำสิ่งต่าง ๆ ได้อย่างอิสระและปลอดภัยในแง่ของการทำงาน ในขณะที่เศรษฐกิจและธรรมาภิบาล เครือข่าย Karura จะให้บริการวัตถุประสงค์ในการทดลองสำหรับAcala

แม้ว่า Mandala จะไม่มีคุณค่าอะไร แต่ก็เป็นสนามเด็กเล่นที่ยอดเยี่ยมในการเตะยางและทดลองขับ(สำนวนว่าเป็นการทดลอง)

# ทดลองขับ Mandala

กู้เงิน aUSD ด้วย BTC เป็นหลักประกัน

Mandala เปิดตัวด้วยคุณสมบัติดังต่อไปนี้:

- สร้าง อัปเดต และจัดการสินเชื่อ aUSD แบบหลายหลักประกัน รองรับการทดสอบ DOT และทดสอบ BTC เป็นหลักประกัน
- An auction module to handle asset liquidation
- A simple oracle implementation with a K’th largest algorithm to tolerate up to K compromised servers
- Built-In decentralized exchange to support instant swaps amongst aUSD, ACA and other supported tokens

Governance is limited to the `Sudo` module for Mandala, while the council set-up is for demonstration purposes only. Check out more in the [Mandala Get Started Guide](https://github.com/AcalaNetwork/Acala/wiki/1.-Get-Started). Or if you can’t wait, [get some test tokens](https://riot.im/app/#/room/#acala-faucet:matrix.org), [jump straight onto the truck](https://apps.acala.network/) and have a drive yourself.

Though there is no reward for validating Mandala, feel free to [run the docker provided](https://github.com/AcalaNetwork/Acala/wiki/4.-Maintainers), or use a hosted service like OnFinality.

Check out [the telemetry](https://telemetry.polkadot.io/#map/Acala%20Mandala%20Testnet) and [the console UI](https://console.acala.network/).

![Image for post](https://miro.medium.com/max/2560/1*yVxtDSo4DnDyfsrEamb2-Q.gif)

# Proof-of-Liveness (PoL) Partners

While the Acala Network will leverage Polkadot’s shared security and do not need dedicated validators itself, it will still require what we call **Proof-of-Liveness (PoL) nodes** to maintain the operation of the Acala network, and propose new blocks to validators for verification.

PoL Nodes will in return receive rewards in kACA in Karura network, and ACA in Acala mainnet. With no particular order, these partners will provide the initial liveness of the Acala network: [OnFinality](https://www.onfinality.io/), [P2P Capital](https://www.p2pcap.com/), and [Stake.Zone](http://stake.zone/).

# The Acala Ecosystem Program

The Acala network is ultimately a community-owned ecosystem. The Acala stablecoin is decentralizedly generated and governed. There are many reasons to choose Acala as the stablecoin provider for your project, and you may have unique questions and needs.

We believe [**the Acala Ecosystem Program**](https://forms.gle/iYPUrNzSWGmyvPUp6) would be a good starting point to form closer collaboration, for us to provide better support to teams integrating with Acala, and co-create incentivize programs, etc. These teams have become the inaugural Acala Ecosystem Program projects: [Chainlink](https://chain.link/), [ChainX](https://chainx.org/), [Dipole](http://www.dipole.tech/), [Plasm Network](https://github.com/staketechnologies/Plasm), [PolkaWorld](https://www.polkaworld.org/), [Subsocial](http://subsocial.network/), and [XanPool](https://www.xanpool.com/).

If you would like to join the Acala Ecosystem Program, submit your interest [here](https://forms.gle/iYPUrNzSWGmyvPUp6).

# Stay Updated with Acala

Website: [https://acala.network](https://acala.network/)  
Twitter: [https://twitter.com/AcalaNetwork](https://twitter.com/AcalaNetwork)  
Medium: [https://medium.com/acalanetwork](https://medium.com/acalanetwork)  
GitHub: [https://github.com/AcalaNetwork/Acala](https://github.com/AcalaNetwork/Acala)

The Acala Stablecoin Project is proudly supported by the Web3 Foundation

<img alt="Image for post" class="t u v ic aj" src="https://miro.medium.com/max/1500/0\*pJgP3IFBAlYbGn11.jpg" width="750" height="300" srcSet="https://miro.medium.com/max/552/0\*pJgP3IFBAlYbGn11.jpg 276w, https://miro.medium.com/max/1104/0\*pJgP3IFBAlYbGn11.jpg 552w, https://miro.medium.com/max/1280/0\*pJgP3IFBAlYbGn11.jpg 640w, https://miro.medium.com/max/1400/0\*pJgP3IFBAlYbGn11.jpg 700w" sizes="700px" />

# About Web3 Foundation

Web3 Foundation funds research and development teams building the stack of technologies that form the basis of the decentralized web. It was established in Zug, Switzerland by Ethereum co-founder and former chief technology officer Dr. Gavin Wood.

For more information on Web3 Foundation, visit [web3.foundation](https://web3.foundation/).

# About Polkadot

Polkadot is the first interoperability protocol that enables blockchain networks of all kinds to work together under the protection of shared security. Applications from decentralized finance and energy to gaming and communications will thrive on Polkadot, forming the basis of digital jurisdictions in Web 3.0. Polkadot is the first project spearheaded by Web3 Foundation.  
For more information on Polkadot, visit [polkadot.network.](https://polkadot.network/)
