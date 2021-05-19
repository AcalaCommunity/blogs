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
- オラクルネットワークで、価格のフィードを取得する。 [こちら](https://wiki.acala.network/build/development-guide/smart-contracts/advanced/use-oracle-feeds)を試してみてください。
- DEX、ステーブルコインのレンディング、リキッドステークのデリバティブなどのプロトコル（例：ステークスしたDOTをリキッドDOTにするなど）

## **🐰🕳 AcalaのEVMについて深く知りたい方は** [**Acala WikiのEVMに関する詳細なセクション**](https://wiki.acala.network/learn/basics/acala-evm/acala-evm-composable-defi-stack)**をご覧ください**

## Try it out at ETHDenver 2021

AcalaはETHDenver 2021でAcala EVMをデビューさせ**Acala EVMを使ってDAppを構築する**または<0>オンチェーン自動スケジューラ機能を備えたAcala EVMを使ってDAppを構築する**というハッカーに3,000ドルを提供しています。</p>

- Acala[**ETHDenver Hacker guide**](https://wiki.acala.network/general/contribution-rewards/ethdenver-hacker)**を探す。</li>
- [**ETHDenver's Bounty Hub**](https://www.ethdenver.com/post/acala)と[**Team Guidelines**](https://www.ethdenver.com/judging)**をチェック</li> </ul>

[ETHDenver 2021でAcalaのEVMを使ってDeFi DAppをPolkadotに対応させてみよう](https://medium.com/acalanetwork/make-your-defi-dapp-polkadot-ready-with-acalas-evm-at-ethdenver-2021-b542090f6af1)

# **高いレベルでのAcala**

初めての方のために説明すると、Acalaは、Polkadotのマルチチェーンネットワークを活用した、スケールに合わせて構築されたEthereum対応の分散型金融（DeFi）プラットフォームです。 Acalaはレイヤー1のインフラを提供するパラチェーンであり、Acalaチームはパラチェーン上にアプリケーションレイヤー全体を構築します。 Acalaのアプリケーションは、ステーブル資産（aUSD）を中心に構築されており、借り入れや貸し出し、合成資産の取引、利息の受け取りなどのエンドユーザー向けのアプリケーションを提供しています。 開発者は、独自のアプリケーションを構築するためのプラットフォームとしてAcalaを活用することができます。

このプラットフォームは、ビットコインのようなクロスチェーン資産に裏付けられた複数の担保を持つステーブルコイン、信頼性の高いステーキングデリバティブ、そして分散型取引所といった一連の金融プリミティブを提供します。 **Acalaのプラットフォームは以下を提供します**

1.  **マイクロガス料金** - Acalaは、前述の「bring your own gas（ガスの持ち込み）」機能との組み合わせで、DeFiユーザーのガスコスト問題を解決します。
2.  **ステークデリバティブL-DOT**（AcalaのDeFiアプリケーションで使用するために、ステーク済のDOTから流動性を放出するリキッドDOT）
3.  **ステーブルコインの貸し借り**（DOT、Bitcoin、L-DOTを主要担保資産とする）
4.  **利回りと利息の獲得**
5.  **分散型取引所**(DEX) での取引
6.  オンチェーン**ガバナンス**
7.  オンチェーン**トレジャリー**
8.  **集約オラクルの価格フィード**のネイティブネットワーク
9.  **オンチェーン・ソブリン・ウェルス・ファンド**がネットワークの未来を支える（[続きを読む](https://medium.com/acalanetwork/building-a-decentralized-sovereign-wealth-fund-6a5a0ae995b1)）
10. **フォークなしで継続的にアップグレード**：Acalaはフォークなしでシームレスにアップグレードできることを覚えておいてください。 つまり、未来は事実上、無限大なのです。 新しいSubstrateパレット（DeFiのプリミティブやランタイムの形をした製品や機能）は、Acalaにスムーズに統合することができます。 Iphone12を手に入れた場合に、手のひらの上で13、14、15+に自動アップグレードされるようなものです。

![投稿画像](https://miro.medium.com/max/3200/0*iHVQdZllz1MxLwuy)

http://apps.acala.network

新しいAcalaのEVMをチェックしていただきありがとうございます。 今後も、Acala EVMの進捗状況や、エコシステムにもたらす様々なメリットについての更なる教育資料を提供していきます。 [Discord](https://discord.gg/vdbFVCH)、[ニュースレター](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc)または以下のチャンネルから最新情報を入手してください。

![投稿画像](https://miro.medium.com/max/2402/0*BvF8sTfeQd4Sc71D.png)

# **Acalaについて**

[Acala](http://acala.network/)は、Polkadotの分散型金融ハブおよびステーブルコインであり、金融アプリケーションの利用や構築を迅速かつ容易にし、取引の効率化と時間の節約を実現します。 マイクロガスコストで運営されているこのプラットフォームは、一連の金融プリミティブを提供しています。これはビットコインのようなクロスチェーン資産に裏付けられたマルチ担保のステーブルコイン、信頼性の高いステーキングデリバティブ、そして分散型取引所で、流動性を解き放ち、金融イノベーションを実現していきます。 Acalaは、金融アプリケーションがスマートコントラクトや内蔵プロトコルを使用するための、事実上のオープンプラットフォームであり、すぐに使えるクロスチェーン機能と強固なセキュリティを備えています。

[Discord](https://discord.gg/vdbFVCH) | [Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) | [All Channels](https://linktr.ee/acalanetwork)
