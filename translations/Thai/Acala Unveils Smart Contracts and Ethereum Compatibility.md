# Acala เปิดตัวสัญญาอัจฉริยะ (Smart contract) และความสามารถในการทำงานร่วมกับ Ethereum สำหรับ Polkadot DeFi

## Cala รองรับ EVM และ Ink แล้วนะ! pallets บน Substrate, enabling Solidity and Wasm-based Smart Contracts for developers

![Image for post](https://miro.medium.com/max/1600/0*-4rCl6SjqDKz7eBh)

โดย Bryan Chen

Polkadot ได้รับการออกแบบมาให้สามารถทำงานกับบล็อคเชนอื่น ๆ เช่น Bitcoin และ Ethereum ได้อย่างง่ายดาย (ผ่านสะพานเช่น Interlay และ RenVM) และเพื่อโฮสต์ห่วงโซ่ที่แตกต่างกันจำนวนหนึ่ง (หรือที่รู้จักกันในชื่ออิสระและปรับแต่งได้) แต่เชื่อมต่อถึงกันเรียกว่า parachains Polkadot เป็นเหมือนห่วงโซ่โครงสร้างพื้นฐานแบบเลเยอร์-0 โดยมอบเลเยอร์ความน่าเชื่อถือพื้นฐานที่มาพร้อมกับความปลอดภัย Proof of Stake (PoS) ที่ใช้ร่วมกันและการสื่อสารข้ามสายโซ่ Parachain chains มีแนวโน้มที่จะเป็น chain-specific chains ที่ปรับให้เหมาะสมสำหรับกรณีการใช้งานและแก้ปัญหาโดเมนเฉพาะ ซึ่ง Acala ครอบครองโดเมนของ Decentralized Finance เราขอเสนอชุด DeFi ดั้งเดิมที่พร้อมใช้งานทันที เช่น stablecoin (aUSD) อนุพันธ์ Stake (เช่น อนุญาตให้คุณแลกโทเค็น (LDOT) บน Staked/locked DOT) และการแลกเปลี่ยนแบบกระจายอำนาจเพื่อขับเคลื่อนนวัตกรรม DeFi ที่มากขึ้น นอกจากนี้เรายังมีโมดูลยูทิลิตี้ทั่วไปแบบโอเพนซอร์ส เช่น Oracle, หลายสกุลเงิน, กรอบงานการตรวจสอบทั่วไปสำหรับทีมที่จะใช้

Substrate-based parachains เช่น Acala จะเพลิดเพลินไปกับ Tech-stack เต็มรูปแบบที่มีให้โดยเฟรมเวิร์กนี้ ตั้งแต่โครงสร้างพื้นฐานทางเทคนิคระดับต่ำ (RPC, รันไทม์ของ web-assembly, การสื่อสารแบบ peer-2-peer เป็นต้น) ไปจนถึงโมดูลระดับแอปพลิเคชันที่เปิดใช้งาน ความสามารถ EVM (Ethereum Virtual Machine) และ Smart Contract ซึ่งหมายความว่าในอนาคตอันใกล้นี้ นวัตกรรมระดับลูกโซ่และความก้าวหน้าทางเทคโนโลยีจะเกิดขึ้นด้วยความเร็วที่ไม่เคยมีมาก่อนในวงกว้าง ความสามารถใหม่จะเป็นแบบ Plug-and-Play ผ่านการอัปเกรดแบบไม่ต้องใช้ส้อมในเครือข่ายที่ใช้ Substrate ทั้งหมดอย่างง่ายดายและต่อเนื่อง (ดูตัวอย่างใน [Substrate Marketplace](https://marketplace-staging.substrate.dev/))

ที่กล่าวว่า Acala ได้เปิดใช้งานความสามารถในการทำสัญญาอัจฉริยะ (Smart Contract) ในรูปแบบต่อไปนี้:

1.  Acala รองรับพาเลท EVM (หรือที่เรียกว่า module แบบ runtime) ซึ่งโดยพื้นฐานแล้วการใช้งาน Ethereum Virtual Machine บน Substrate เพื่อให้สามารถปรับใช้และรันสัญญา Solidity บน Acala ได้
2.  Acala ยังสนับสนุน ink อีกด้วย! พาเลทสัญญา ซึ่งเปิดใช้สัญญาสมาร์ทเนทีฟของพื้นผิวที่ใช้ Wasm (Web Assembly) ซึ่งเขียนด้วยภาษา Rust

การอัปเดตนี้ขับเคลื่อนโดยทั้งความก้าวหน้าทางเทคนิคและความสนใจของชุมชน Acala กำลังช่วยโปรโตคอลจำนวนหนึ่งสำรวจการปรับใช้ DeFi ข้ามสายโซ่บน Polkadot ซึ่งเป็นกลไกที่เราจะแกะกล่องในบทความนี้ และ Smart Contracts ก็เป็นหนึ่งในช่องทางสำคัญในการสำรวจอย่างแน่นอน ต่อจากนี้ Acala จะร่วมมือกับ [Parity](https://www.parity.io/) และอื่น ๆ ในระบบนิเวศอย่างแข็งขันมากขึ้น เช่น [Moonbeam](https://moonbeam.network/), [Plasm](https://www.plasmnet.io/) และ [Edgeware](https://edgewa.re/) และมีส่วนร่วมใน EVM และการพัฒนาสัญญาอัจฉริยะ

# ตอนนี้เราจะเจาะลึกในหัวข้อต่อไปนี้:

1.  Cross-chain Liquidity ผ่านการ Bridge
2.  วิธีการปรับใช้บน Polkadot
3.  วิธีการปรับใช้บน Kusama
4.  วิธีการปรับใช้บน Acala
5.  สถานะปัจจุบันของ Smart Contracts บน Polkadot

# Cross-chain Liquidity ผ่านการ Bridge

Bridges are interoperable technology to cross assets and messages between two economically sovereign and technologically diverse chains e.g. between Polkadot and Ethereum or Bitcoin. There are different flavors of bridges ranging from centralized and trusted to more decentralized and trustless.

1.  **Custodial solutions**: using multi-sig or Proof of Authority (PoA) types of setup, they are relatively easier to implement and are available to use right now. [ChainX](https://chainx.org/) as Bitcoin bridge and [ChainSafe](https://chainsafe.io/) as Ethereum bridge are examples of this type, with roadmaps to become more decentralized over time.
2.  **Trustless solutions**: using economic and/or cryptographic guarantees to transfer assets to/from two blockchains; they are trustless, but could be expensive to users, and also are still under research and development due to technical challenges of its trustless nature. [Interlay](https://medium.com/interlay/bitcoin-on-polkadot-proof-of-concept-for-trustless-bridge-shipped-6fb8e549bef0) as a Bitcoin bridge and [SnowFork](http://www.snowfork.com/) and [Darwinia](https://darwinia.network/) as an Ethereum bridge are examples of this type.
3.  **Hybrid Custodial/Trustless solutions**: then there’s the [RenVM](https://renproject.io/) solution that is permissionless with great UX and popularity with a clear pathway towards decentralization, but right now much trust has been placed on the Ren team.

Acala is neutral with regards to approaches to bridge solutions, as different flavors of bridges may satisfy different user preferences of trustlessness, convenience and costs, and there are good reasons for various types of bridges to co-exist and serve various needs.

# Deploying on the Polkadot Relay Chain

As mentioned, Polkadot is a Layer-0 cross-chain infrastructure chain (called the [Relay Chain](https://wiki.polkadot.network/docs/en/learn-architecture#relay-chain)). Applications and protocols hence cannot be deployed directly on the Relay Chain but rather via the following mechanisms provided as fabrics of the Polkadot network, each with its own trade-offs:

1.  **Deploying as a parachain** — This option has the highest degree of customizability and flexibility both technically and economically. It has more ‘permanent’ access (within the parachain lease period) to Polkadot’s shared security and cross-chain communication facility. It does have a higher cost to set up, and require much more effort to bootstrap and maintain the network as well as the community. You can get a taste of this by [exploring Acala](https://github.com/AcalaNetwork/Acala/wiki/1.-Get-Started).
2.  **Deploying as a parathread** — it’s similar to parachain technically, but uses a pay-as-you-go model for security and communication access, hence less overhead upfront and cheaper to run. If a chain cannot get a parachain slot, it can fall-back to parathread to continue its operations.
3.  **Deploying as a DApp on an active parachain/parathread** — for teams who want to access the Polkadot ecosystem but don’t want to build and maintain a blockchain, or who want to try things out without much upfront commitment, then deploying on an existing parachain might be a good option. Especially for DeFi related DApps, you can treat Acala as a landing pad (such as in [Ren’s case](https://medium.com/acalanetwork/bringing-btc-to-polkadot-acala-x-ren-e7959855d5aa?source=collection_home---4------6-----------------------).) and a technical-know-how Polkadot-buddy when exploring the space.

Apart from technical and economic considerations, one shall also think of composability. The degree and sophistication of composability may vary depending on where you land — DApps on one parachain would naturally enjoy a higher degree of composability within that chain (read Ren’s integration [here](https://github.com/AcalaNetwork/Acala/wiki/T.-Cross-chain-DeFi#ren)), cross-parachain DApps may have reduced composability and atomicity of transactions (read Laminar’s integration [here](https://github.com/AcalaNetwork/Acala/wiki/T.-Cross-chain-DeFi#laminar)), and bridges may have even lower composability as they are mostly focused on value transfers and certain specific message passing across designated blockchains.

# Deploying on Kusama’s Relay Chain

[Kusama](http://kusama.network), similar to Polkadot, is a Layer-0 cross-chain infrastructure chain with a core [Relay Chain](https://wiki.polkadot.network/docs/en/learn-architecture#relay-chain) that provides security and interoperability. Kusama is meant to be a development environment for teams preparing for deployment on Polkadot, or for teams who want to build exclusively on Kusama for lower economic barriers to parachain slots and for faster governance cycles. Developers have the same options with Kusama as they do with Polkadot, with a few caveats:

1.  **Deploying as a parachain** — Teams can build a parachain on Kusama for three primary reasons. First, parachains can be deployed to Kusama after passing testing on the Westend testnet in order to fine-tune their technology before a full deployment to Polkadot. Some teams, Acala included, will choose to operate parachains on both Polkadot and Kusama to serve both communities. Third, teams (e.g. new startups) may also choose to stay exclusively on Kusama if the cost for a Polkadot parachain slot is out of reach or if they prefer the risk-taking and fast-moving nature of Kusama. The Kusama parachain option is also customizable and flexible both technically and economically.
2.  **Deploying as a parathread** — Kusama will have the same parathread functionality as Polkadot, which is a pay-as-you-go model for security and communication access, leading to less overhead and expense to run. One tradeoff is that parathreads come with less frequent block submissions to the Relay Chain, so it may suit some use cases better than others.
3.  **Deploying as a DApp on an active parachain/parathread** — DApps can be built on Kusama parachains or parathreads. DeFi DApps for example can be built on Acala’s Kusama Network, as well as many other use cases like gaming, communications, social media, or DAOs.

In the next sect we will explore different ways to deploy on Acala parachain.

# Deploying on the Acala Parachain

You can treat Acala as the DeFi landing pad on Polkadot and Kusama, and your technical-know-how builder-buddy. There are currently three ways you can deploy on Acala:

1.  **Deploy runtime modules (aka pallets)** — this enables the highest level of customizability, and access to Acala’s chain logic for a more sophisticated integration. It does not have the fail-safe sandbox environment that smart contracts enjoy, hence it requires security audits and requires governance permission. It suits better for infrastructure and common-good protocols. The [RenVM bridge module](https://github.com/AcalaNetwork/Acala/tree/master/ecosystem-modules/ren/renvm-bridge) is a good example of this. A brand new account with only freshly minted renBTC, can perform any transactions on Acala without needing a fee token. Thanks to Acala’s FlexFee feature, tokens like renBTC are integrated natively as one of the default fee tokens alongside ACA, aUSD and DOT.
2.  **Deploy Solidity smart contracts** — for those who want to migrate part or all of their existing Solidity smart contracts to Polkadot without re-writing all the code, this can be a good starting point. As an example, some teams would use a bridge to cross their tokens from Ethereum to Polkadot, then deploy on Acala for faster, cheaper transactions and better user experience.
3.  **Deploy ink! smart contracts** — this is Substrate’s native, Rust-based Wasm smart contract, read more on how it compares to EVM [here](https://substrate.dev/docs/en/knowledgebase/smart-contracts/ink-fundamentals).

As a disclaimer, smart contract modules are close to but not yet (to Acala’s standard) production-ready, and we will be working closely with Parity and others in the ecosystem to finalize them. We outline the caveats and current state of the development in the next section.

# The Current State of Smart Contracts

## EVM

While Solidity and EVM-compatible contracts can be deployed and run on Substrate-based chains like Acala, much of the tooling is still being developed so that it’s compatible with existing development tools such as Truffle and Remix etc. SDKs are also being developed to be compatible with existing web3.js and other libraries. Acala will also focus on improving the composability of smart contracts and runtime modules to accelerate cross-chain DeFi innovation.

## Ink! Smart Contracts

Rust-based ink! smart-contract language is still under development, as are its development tooling (cargo-contract and [Redspot](https://github.com/patractlabs/redspot) — Truffle for Ink!) and SDKs (polkadot.js).

# Next Steps

Acala now supports EVM with the [Frontier](https://github.com/paritytech/frontier) Substrate-Ethereum compatibility layer. We can now run unmodified Ethereum DApps. Next, we will be deploying more complex (real-life) Solidity contracts, testing out tooling supports including Metamasks, and implementing pallet (runtime module) integration to improve compatibility, and to become compatible with ERC20 and other token standards.

Consider this your official invitation to [**Build with Acala**](https://github.com/AcalaNetwork/Acala/wiki/U.-Build-with-Acala), where we support and help teams create valuable cross-chain DeFi projects with Polkadot and Kusama.

# Join Us

[Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launches on Polkadot and Kusama, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot that makes it fast and easy to use or build financial applications, improving trading efficiency and saving valuable time. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.
