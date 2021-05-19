# **Acala、Polkadot上のDeFi用Acala EVMをローンチ｜Sabstrateの機能に制限のないEthereumとの互換性を実現**

![投稿画像](https://miro.medium.com/max/6000/1*FNYYia98MytjFEU1Dtuzqw.png)

## Acala EVMはEthereumの長所を活かしつつ、Substrateの可能性を最大限に引き出し、Bring Your Own Gasやオンチェーンの自動スケジューリングなど、コンポーザブルでシングルウォレットのAcala-EVM-Substrate-WASMのエクスペリエンスを提供します。

Acalaのエンジニアリングチームは、Acala EVMをカスタムメイドしてローンチしました！ Polkadotのエコシステムにとって斬新なこのイノベーションにより、AcalaはSolidity、Substrate、Web3の開発者に、単一のウォレットでシームレスに完全なフルスタック（Acala+EVM+Substrate+WASM）のエクスペリエンスを提供することができます。 また、Acala EVMは、EVMとSubstrateのランタイム（別名：パレット）にプロトコルのコンポーザビリティをもたらし、開発者は卓越したツールのサポートを受けて、Acala上でDAppsを構築・デプロイすることができます。

イーサリアムがビットコインにはできないことを可能にし、それが多くの新しいイノベーションを生み出したように、SubstrateとPolkadotはイーサリアムとは決定的に異なり、EVMのサンドボックス外で多くの新しいチェーンレベルのイノベーションを生み出すでしょう。 私たちはSubstrateの力を確信しており、Polkadot上のEthereumを単に再配置するのではなく、Substrateの可能性と持続可能性を最大限に引き出すためにAcala EVMを構築しました。

# **The Acala EVM**

## **コンポーザブルなDeFi環境**

Acala EVMにデプロイされたスマートコントラクトDappsは、DOT、ACA、aUSD、renBTC、XBTCなどのネイティブおよびクロスチェーンのアセットを直接使用することができます。 EVMに配置されたERC-20トークンは、ランタイムレベルで利用可能にしたり、DEXにリストしたり、（ガバナンスの承認を得て）ガス料金トークンとして使用することもできます。 これは、例えば、AmpleforthがAcala EVM上にAMPLコントラクトを展開し、ネイティブトークンとして利用できるようにすることで、取引手数料の支払いに利用したり、当社のDEXに直接上場することができることを意味します。

コンポーザビリティの概念を初めて知った方 A16zは、[4 Eras of Blockchain Computing](https://a16z.com/2018/12/16/4-eras-of-blockchain-computing-degrees-of-composability/#:~:text=A%20platform%20is%20composable%20if,more%20rapid%20and%20compounding%20innovation.)で非常にうまく表現しています。Degrees of Composability</0>です。

Acalaの共同設立者兼CTOブライアン・チェン氏が、AcalaにUniswapを導入して2分以内に取引を実行した際のAcala EVMの使用例を紹介していますので、ご覧ください。

## **Acala EVMの完全にコンポーザブルなDeFiプリミティブ**

- **Bring your own gas**：ほぼ全てのトークンを使用可能に- Acalaに統合されたネイティブトークンとクロスチェーントークンはガスの支払いに使用できるようになります。 ライブでは以下のようになります：_DeFiで遊び始めるためにAcalaにラップETHを送ってみましょう ETHをブリッジ経由でAcalaに送り、ラップされたETHをガス料金として使用して、Acala DeFiアプリですぐにデプロイを開始することができます。 わざわざACAを探しに行く必要はありません_
- サブスクリプションや定期的な支払いなどのユースケースを可能にする**オンチェーンの自動スケジューラー** お試しは[こちら](https://wiki.acala.network/build/development-guide/smart-contracts/advanced/use-on-chain-scheduler)または以下の6分間のデモをご覧ください。

- **ネイティブトークンとクロスチェーントークン**がERC20で利用可能：DOT、ACA、aUSD、XBTC（ChainXから）、LDOT（リキッドステークDOT）、RENBTCなど
- オラクルネットワークで、価格のフィードを取得する。 Try it [here](https://wiki.acala.network/build/development-guide/smart-contracts/advanced/use-oracle-feeds).
- Protocols such as DEX, stablecoin lending, and liquid staking derivatives (e.g. liquid DOT for your staked DOT)

## **🐰🕳 For a deep dive on the Acala EVM, check out the** [**Acala Wiki’s in-depth EVM section**](https://wiki.acala.network/learn/basics/acala-evm/acala-evm-composable-defi-stack)**.**

## Try it out at ETHDenver 2021

Acala is debuting the Acala EVM at ETHDenver 2021, offering $3k USD for hackers to “**Build a DApp Using the Acala EVM**” or “**Build a DApp Using the Acala EVM with the On-Chain Automatic Scheduler Function**”.

- Find Acala’s [**ETHDenver Hacker guide**](https://wiki.acala.network/general/contribution-rewards/ethdenver-hacker)**.**
- Check out [**ETHDenver’s Bounty Hub**](https://www.ethdenver.com/post/acala) and [**Team Guidelines**](https://www.ethdenver.com/judging)**.**

[Make Your DeFi DApp Polkadot-Ready with Acala’s EVM at ETHDenver 2021](https://medium.com/acalanetwork/make-your-defi-dapp-polkadot-ready-with-acalas-evm-at-ethdenver-2021-b542090f6af1)

# **Acala at a High Level**

If you’re new here, Acala is an Ethereum-compatible decentralized finance (DeFi) platform built for scale, leveraging Polkadot’s multi-chain network. Although Acala is a parachain providing layer 1 infrastructure, the Acala team has also built out an entire application layer on top of the parachain. Acala’s applications are built around a stable asset (aUSD) and offers end-user applications such as borrowing, lending, synthetic asset trading, and interest earning, all executed extremely fast with inexpensive gas fees. Developers can also leverage Acala as a platform on which to build their own applications.

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
