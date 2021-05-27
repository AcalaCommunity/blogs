# Acalaセキュリティ監査

![投稿画像](https://miro.medium.com/max/8000/1*yhydywHe1k2421hd6xqhFQ.jpeg)

Acalaでは、企業ではなく個々のユーザーが自分たちのファイナンスを管理する必要があると考えています。 私たちの使命は、Web 3.0の金融アプリケーションをサポートし、育成することです。 よりオープンで公平な財務の未来は、当社のDeFi最適化されたスマートコントラクトプラットフォームとAcalaのプロトコルである分散型ステーブ定コインを通じて可能にしたいと考えていますそれはトラストレスな流動性提供と分散型取引所です。

とはいえ、Acalaのブロックチェーンとプロトコルのセキュリティが私たちの最優先事項です。 私たちは、安全で信頼性の高いプラットフォームと関連プロトコルを開発するために多大な努力を払ってきました。また、私たちのコードベースを監査するために、この業界で最も優れた企業と契約しました。

![投稿画像](https://miro.medium.com/max/1730/1*hKvzkJVXDmSA9OU7NhFLuA.jpeg)

監査の範囲には、エコシステムモジュールRenVMを含むAcalaのすべてのランタイム実装が含まれていました。 Acalaが依存するORMLモジュールと、AcalaのDAppのフロントエンドインターフェイスを管理しています。 これまでSRLabsとスローミストは監査を完了し、Trail of Bitsの監査は2021年1月に開始される予定です。

# レポート & 修正

SRLabsの監査では、0件のクリティカル、1件のハイ、7件のミディアム、2件のローレベルの問題が見つかりました。

SlowMistの監査では、0件のクリティカル、0件のハイ、1件のミディアム、1件のローレベルの問題が見つかりました。

ハイレベルの問題は、監査の時点ではまだ実施されていない計画されたタスクでした。 現在、ベンチマークを完了し、全ての[外在的](https://substrate.dev/docs/en/knowledgebase/learn-substrate/extrinsics)課題（署名済み/未署名のトランザクションや、ブロックに含まれるがゴシップにならない情報）に対する処置を行いました。

他のすべてのネットワークセキュリティ関連の問題は、監査役によって対処され、レビューされています。 アプリケーション関連の問題が2つあります(SRLabsのレポートでは#5と#8)。DeXフロントランニングなどの一般的なDeFiの問題です。 満足のいく解決策が得られていません 安全パラメータを設定することで、リスク管理の観点から取り組んでいます。 それ以外は シミュレーションに基づく市場ストレステストを利用した更なる経済監査を求めており、規模と価値の拡大により脆弱性と市場リスクを評価することができます。

SRLabsとSlowMistからの完全なレポートは [こちら](https://github.com/AcalaNetwork/Acala/tree/master/audit)

# 未来へ向けて

監査は、セキュリティの確保とリスク管理における当社の努力の一部に過ぎません。 Acalaのランタイムコードベースはすべて監査され、ジェネシスの場合、すべてのバランスとガバナンスの決定は公的に検証可能になります。 [Bug Bounty Program](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#runtime-bug-bounty) はコードベースを安全に保つための重要な部分でもあります。 開発者にコードを調べて脆弱性を報告するよう勧めます。 私たちは、透明性、時間、価値がネットワークとプロトコルのセキュリティの真のテストであると信じています。今後も警戒しつつ注視してフィードバックを行い、Acalaを誰にとってもより安全でセキュアなものにするためにご協力ください。

# 参加しませんか

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

Acalaのパラチェーンのローンチの進捗状況を知りたい方は、[Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc)をご購読ください。

# Acalaについて

[Acala](http://acala.network/)は、Polkadotの分散型金融ハブであり、高速で使いやすい金融アプリケーションを誰もが利用できるようにします。 このプラットフォームは、一連の金融プリミティブを提供しており、ビットコインなどのクロスチェーン資産に裏付けられたマルチ担保のステーブルコイン、信頼性の高いステーキングデリバティブ、そして分散型取引所によって、流動性を解き放ち、金融イノベーションを実現します。 Acalaは、金融アプリケーションがスマートコントラクトや内蔵プロトコルを使用するためのオープンプラットフォームであり、利便性の高いクロスチェーン機能とセキュリティ、財務の最適化を備えています。
