# Acalaのエクストリーム・テスト・シミュレーションから学んだこと

## Acalaによる3週間のテストネットキャンペーンが終了し、カナリア・ネットワークの重要性が浮き彫りになるとともに、ネットワークの技術的な改善にもつながりました

![投稿画像](https://miro.medium.com/max/1600/1*lGVbzGOgp5M3DqCPtAds8A.jpeg)

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
- キーパーの非効率性&流動性の低下

## 以下の改善を実施しました：

- **オラクル・オペレーションのサービス品質：** オラクルのトランザクションは優先され、常にブロックに含まれる為に価格フィードは常に最新でネットワークトラフィックの影響を受けません
- **オートリクイデーター** [オフチェーンワーカーの使用](https://www.parity.io/substrate-off-chain-workers-secure-and-efficient-computing-intensive-tasks/)：キーパーのような外部アクターがMakerのようなプロトコルで必要とされるのは、Ethereumや同様の技術がブロックチェーンノード上で安全でセキュアなオートスケジューラーを提供できないからに他なりません Acalaは全てのブロックのローンポジションを効率的に評価できるオートリクイデーターを導入しました
- **DEXとオークションのハイブリッドな流動化メカニズム：** オークションでの価格の非効率性を避けるために、価格とスリッページが良好な場合、システムはDEXでコラテラルを自動的に流動化します
- **スループットの高さと特殊性：** Acalaのスループットは1000 tpsと最適化されていません。Polkadotのマルチチェーンでは、各シャード/パラチェーンはそのユースケースに合わせて最適化されていると思われます。 例えるなら、AcalaはDeFi領域全般に最適化された金融シャードであり、別のチェーンはゲームやペットの繁殖などの用途に特化したものになるでしょう。 Polkadotの実際のスループットは、1000tpsに接続されているシャード/パラチェーンの総数を掛けたものになります

キャンペーン期間中、Acalaは「ブラックサーズデー」を想定した訓練を行い、価格変動が激しく、リスクの高いローンポジションを清算してシステムを緊急停止させるというシミュレーションを行いました。 高負荷の中、システムは期待通りに動作し、最終的には全てのローンが処理され担保がユーザーに返却されました

📉 14,400+ ローンを清算

⚡️ 計137万ドルの資産が清算

# クロスチェーン流動性の力

Acalaは、Polkadotのマルチチェーンユニバースのファイナンスハブです。 複数の担保を持つステーブルコイン、信頼性の高いステーキングデリバティブ、分散型取引所など、一連の金融プリミティブを提供しています。 各プリミティブは、AcalaのDAppを介してエンドユーザーに直接提供され、また、他のDAppが構築するためのSDKとしても提供されます。 相互に接続され、自律的で洗練された、クロスブロックチェーンの金融エコシステムが出現しつつあると考えています。

そしてAcalaは、RenやLaminarと統合し、クロスチェーンリクイディティの力を明示する事に成功しました。

₿ 1,403 renBTC がミント

👨‍🌾 140万ドル相当のrenBTCがDeXで取引され、550万ドルが融資

🌈 430万ドル相当のaUSDがLaminarの合成資産（FX、金、合成BTC、ETH）の証拠金取引に利用

AcalaのクロスチェーンDeFiのユースケースについては[こちら](https://github.com/AcalaNetwork/Acala/wiki/T.-Cross-chain-DeFi)をご覧ください。また、私たちのフレームワークやDeFiプリミティブ、SDKを使って、次のキラーDeFiプロジェクトを作りましょう！ 私たちが提供するのはプロダクショングレードであり、プロダクションレディです。 また、最近行われたKusamaのHackusamaイベントに私たちは教育的パートナーとして参加しました。もっと知りたい方は[こちらへ](https://medium.com/acalanetwork/hackusama-ea1ddf3e945a)。

# 参加する

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

Acalaのパラチェーンローンチに向けた進捗状況を知りたい方は、[Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc)をご購読ください。
