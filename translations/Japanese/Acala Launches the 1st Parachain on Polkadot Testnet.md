# AcalaはPolkadot Testnetで最初のパラチェーンをローンチします

![投稿画像](https://miro.medium.com/max/8000/1*IGXwgFXEA7viM8upZgcw2g.jpeg)

AcalaをPolkadotのパラチェーンとしてローンチする為の重要なマイルストーンに到達しました。[Rococo - Polkadotのパラチェーンテストネット](https://medium.com/polkadot-network/introducing-rococo-polkadots-parachain-testnet-e3e67fc40b56)の最初のパラチェーンとしてAcala Mandala PC1 (Parachain Candidate 1) テストネットをローンチしました。

Rococoは、[Cumulus](https://wiki.polkadot.network/docs/en/build-cumulus)によるパラチェーンコンセンサスと共有セキュリティ、およびHRMP（Horizontal Relay-chain Message Passing）によるクロスチェーンコミュニケーションを実現します。 HRMPでは、後に[XCMP](https://wiki.polkadot.network/docs/en/learn-crosschain)(Cross-chain Message Passing)によってパラチェーン間で直接通信するための足がかりとして、リレーチェーンを介してクロスチェーン・メッセージをルーティングする必要があります。

Acala Mandala PC1を使えば

- **クロスチェーンコンセンサスとメッセージパッシングを使用して、AcalaのフルDeFiスイート**（ステーブルコイン、ステーキングデリバティブ、DeX）をテスト
- [Cross-Consensus Message (XCM) フォーマット](https://github.com/paritytech/xcm-format)の実装をさらに発展させ、特に我々が主導していた**Cross-chain fungible token standard**を具体化しました。 ドラフト規格[こちら](https://github.com/w3f/PSPs/blob/master/PSPs/drafts/psp-3.md)＆PoCパレットの実装[こちら](https://github.com/open-web3-stack/open-runtime-module-library/tree/rococo/xtokens)。
- **Acala Collatorノードのテスト**と報酬スキームの実装
- **クロスチェーン・インテグレーションのテスト** **Laminar、Plasm、Interlayなどの他のパラケイン**との統合
- Homaプロトコルの**trustless staking bridge to Relay-chain**を実装する。

# Parachain Developer Community

パラチェーンの開発者コミュニティでは以下のように共有しています。

- **Sabstrateベースのチェーンをパラチェーンにする**、Cumulusを[ここ](https://github.com/AcalaNetwork/Acala/pull/362)に統合してノードを[コレーター](https://wiki.polkadot.network/docs/en/maintain-collator)にすることも含みます。
- **クロスチェーン・ファンジブル・マルチ・トークン・トランスファー実装** - 'xtoken' pallet [こちら](https://github.com/open-web3-stack/open-runtime-module-library/tree/rococo/xtokens)。 これにより、既にRococoとMandala PC1の間でROC（Rococoのネットワークトークン）の授受が可能になっており、これを採用したり、同じ規格を使用している他のパラチェーンは、相互にトークンを授受することができます。

# 次の情報

Mandala PC1については、Rococoの最新バージョンへの対応、新機能の展開、他のパラチェーンとの統合サポートのために、予告なしに何度もリセットされることがあります。 Mandala Parachain Candidateの今後の主な展開：

- **XCMパレットの開発を継続する** Parity、Web3 Foundation、およびコミュニティの他の人々と共に、生産可能な状態に向けて開発します。
- **Acalaのステーキングの有効化** Acala Collatorノードの報酬/スラッシュ
- **他のパラチェーンとの広範なクロスチェーン通信テスト**を行い、例えば、単独で実装されていたユースケースの一部を可能にし、マージン取引の基本通貨としてaUSDをLaminarにクロスさせたり、決済手段としてaUSDをPlasmネットワークにクロスさせたりします。
- **Homa ステーキングデリバティブ (LDOT) リレーチェーンブリッジの有効化**KusamaとPolkadotのための信頼性の高いリキッドステーキングをローンチ時に準備できるようにします。

# ローンチ

RococoとMandalaの他にも、カナリア・ネットワークであるKusamaでKaruraをパラチェーン機能が有効になった時点でローンチし、その後AcaraをPolkadotでメインネットをローンチします。 Acalaは、KaruraのAcalaの2つのネットワークを運営し、KusamaとPolkadotの両エコシステムにDeFiインフラと流動性を提供します。 今後は、パラチェーンオークションの準備をしてスロットを確保し、2つのネットワークでローンチする予定です。 **Subscribe** [**こちら**](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) **Acalaパラチェーンのオークションや各種リリース関する最新情報をお届けします。</p>

# Acalaについて

[Acala](http://acala.network/)は、金融の安定性、流動性、アクセス性をメインストリームにもたらすというビジョンを持つ、世界初の分散型金融コンソーシアムです。 Acala Networkは、Polkadotのエコシステムとその先を見据えたクロスチェーンファイナンスのハブです。 ビットコインのようなクロスチェーン資産に裏付けられたマルチ担保のステーブルコイン、信頼性の高いステーキングデリバティブ、分散型取引所など、一連の金融プリミティブを提供し、流動性を解き放ち、金融イノベーションを実現します。 金融系のdAppsがスマートコントラクトや内蔵プロトコルを使ってデプロイするためのオープンプラットフォームであり、クロスチェーン機能、セキュリティ、金融の最適化が可能です。

**参加する**

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

![投稿画像](https://miro.medium.com/max/1500/0*YTeYSsHAVjOBCZu8.jpeg)

AcalaはWeb3 Foundationの助成金を受けています。
