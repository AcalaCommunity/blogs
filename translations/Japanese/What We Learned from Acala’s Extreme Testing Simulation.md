# Acalaのエクストリーム・テスト・シミュレーションから学んだこと

## Acalaによる3週間のテストネットキャンペーンが終了し、カナリア・ネットワークの重要性が浮き彫りになるとともに、ネットワークの技術的な改善にもつながりました

![Image for post](https://miro.medium.com/max/1600/1*lGVbzGOgp5M3DqCPtAds8A.jpeg)

By: [Bette Chen](https://medium.com/u/8d475d21e811?source=post_page-----5ef5769a0902--------------------------------)

8月17日、3週間のテストネットキャンペーンであるAcala [Mandala Fest Season #3](https://medium.com/acalanetwork/acala-mandala-festival-season-3-d0a6f155c154)が無事終了しました。 参加者に報酬を提供しながら、高負荷や過酷な状況下でシステムやプロトコルをテストすることで、開発の進捗状況をコミュニティにアピールすることができました。

コミュニティからのサポートと熱意には非常に圧倒されました。 統計データは以下の通りです：

✅ 14,500 + 新規アカウント

⛓️ 140,000 + 意義のあるトランザクション

💰 5200万ドルのLTV

💲 2500万ドルのaUSD発行

**受賞のハイライトは以下の通りで全結果は[**こちら**](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#season-3-prize-giving)に掲載されています**。

😎 第1週目の受賞者は10,525名の応募者の中から2,105名のユーザーが選ばれました

[⌛](https://emojipedia.org/hourglass-done/) 第2週目の受賞者は平均リターン24,200%のトップ10トレーダーに贈られました

🌋第三週目の受賞者は200人に

✍️ 10人のブロガーが受賞

🐞 45人のバグハンターが受賞

🤖️ 1人コードバウンティが受賞

また、システムや設定の再確認や改善につながったものなど、数多くの貴重な知見を得ることができました。

# カナリアネットワークの重要性

従来のブロックチェーン開発は、テストネットとフルプロダクション環境のみで構成されていました。 しかしながら、その方法では私たちは経済状況が万全でない限り適切なテストできない事を意味します。 テストネット「Mandala」のキャンペーンによるインセンティブイベント（主に参加者のラッキードロー）においては、機能性や使い勝手を大々的にテストすることはできても、Mandalaのようなその状況で価値のないテストネットでは、経済的なダイナミクス、流動性の効率性、リスク許容度を十分に検討することができないことが明確になりました。

Polkadotのカナリア・ネットワーク[Kusama](http://kusama.network)と同様に、Acalaは[Karura](https://github.com/AcalaNetwork/Acala/wiki/1.-Get-Started#acala-trilogy-networks)のカナリアネットワークを実装しています。 どちらのネットワークも実質的な経済価値を有していますが、プライマリーネットワーク（ここではAcala）の経済価値よりも低いものとなります。 Karura Networkは、[KAR](https://github.com/AcalaNetwork/Acala/wiki/V.-ACA-&-KAR)ネイティブネットワークトークンを保有することで一定の経済的価値を表しています。このネットワークは、Kusumaネットワーク上でパラチェーンとしてローンチされ、KSMをステーブルコイン・クレジットラインの担保として受け入れるなど、Kusamaエコシステムに金融プリミティブを提供します。

# ブラックサーズデー・シミュレーションの教訓 - 流動性の重要性

私たちは今、分散型（ブロックチェーンベース）の金融システムの金融リスクの許容範囲は、大部分が基礎となる台帳の容量と技術的制約によって決定されるという認識を持っています。 MakerDAOの3月12日の「ブラックサーズデー」事件を引き起こした根本的な問題については[こちら](https://medium.com/acalanetwork/regaining-confidence-in-decentralized-stablecoins-bd98ba8e3c83)を参照してください。

- 基盤となるネットワークのパフォーマンスのボトルネック
- リスクの高い担保付ローンやCDPの流動化の非効率性
- キーパーの非効率性＆流動性の低下

## 以下の改善を実施しました：

- **オラクル・オペレーションのサービス品質：** オラクルのトランザクションは優先され、常にブロックに含まれる為に価格フィードは常に最新でネットワークトラフィックの影響を受けません
- **Auto liquidator** using [Off-chain Workers](https://www.parity.io/substrate-off-chain-workers-secure-and-efficient-computing-intensive-tasks/): external actors like Keepers are required in protocols like Maker only because Ethereum or similar technology cannot provide a safe and secure auto-scheduler on a blockchain node. Acala implemented an auto-liquidator that can efficiently assess loan positions in every block.
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
