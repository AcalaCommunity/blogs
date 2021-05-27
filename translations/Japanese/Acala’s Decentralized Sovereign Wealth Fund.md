# Acala社の分散型ソブリン・ウェルス・ファンド - 次世代DAO & アンフォーク AUM

By [Joe Petrowski](https://medium.com/u/9f4b86fbf09a?source=post_page-----80f8c23d8f27--------------------------------) & [Bette Chen](https://medium.com/u/8d475d21e811?source=post_page-----80f8c23d8f27--------------------------------)

**TLDR:** Acalaは、オンチェーンの分散型Sovereign Wealth Fund（dSWF）とガバナンスによって、経済的・統治的（意思決定）な主権を獲得する次世代DAO - DAO3.0です。 dSWFの資産は基本的には運用目的資産であり、コードや流動性、そしてコミュニティをフォークすることはできても、AUMをフォークすることはできません。

![Image for post](https://miro.medium.com/max/1600/1*tG3vPiETDyoJgt1aC_5ygg.jpeg)

PolkadotとSubstrateは、社会の組織や意思決定の新しい形の基盤となります。 Acalaは、Substrateのガバナンスおよび財務管理機能と、Polkadotのクロスチェーンメッセージングを活用して、分散型のソブリンファンドを設立しています。 この基金により、Acalaチェーンはパラチェンスロットを確保し、最初の資金調達が終了した後も開発を続けることができます。

分散型ソブリン・ウェルス・ファンドの仕組みを説明する前に、まず従来の意味を説明します。 多くのオープンファイナンスコンポーネントと同様に、分散型バリアントは伝統的な金融にそのルーツを持っています。

一般的に、輸出量の多い国は、黒字と通貨の不均衡を管理するためにソブリンファンドを設立することが多々あります。 国が商品を輸出すると、例えば米国ドルのような外国の通貨が入ってきます。 これは、消費者はそれぞれの現地通貨で購入するからです。 しかし、輸出国は自国の労働者に自国通貨で給与を支払う必要があります。 この場合、一般的には、米ドルを売って市場で自国通貨を買うか、自国の通貨を増刷するかの2つの選択肢があります。 中央銀行や政府関係者にとって、前者はあまり好ましいものではありません。自国通貨の価値を受け取る通貨よりも相対的に高めてしまうため、将来の収益の価値が下がってしまうからです。 両方のオプションを組み合わせて使用することもできますが、外貨から自国通貨への換算を最小限に抑えたいと考えるでしょう。 では、その資金をどう扱うべきなのでしょうか？ ソブリン・ウェルス・ファンドは、国家が運営するファンドであり、外貨や貴金属、株式、債券、不動産などの資産を保有しています 。

政府が運営する投資ファンドには、汚職や放埓な議員が多いようです。 一方で、政府系ファンドの中には国民に真の価値を提供しているものもあります。1兆ドル以上の価値を持つノルウェーのファンドは、国民全員に年金を提供しています。

分散型のソブリン・ウェルス・ファンドは、国民に価値を提供する手段を提供しますが、ブロックチェーンが可能にする透明性と正式な論理への厳格な遵守を備えています。 さらにその先も考えられます。 一般的なウェルスファンドは価値を高めることのみを目的としていますが、多くのトークンが_utility_を持つネットワークでは、その保有量に応じて他のブロックチェーンネットワークの機能にアクセスすることも可能です。

# ソブリンエンティティとしてのブロックチェーン

この話題は、「ブロックチェーンは主権を持つことができる」という概念を中心に展開されます。 ソブリンは、代理権や意思決定能力、そしてそれを行使する力の形態を意味します スマートコントラクトのようなブロックチェーンのサブエンティティには限定的なエージェンシーがありますが、ブロックチェーン自体にはエージェンシーも主権もありません。 例えば、「Bitcoin on Ethereum」では、Ethereum上のコントラクトは一部のBitcoinを所有できますが、ネットワークとしてのEthereumは所有できません。

Substrateのガバナンスプリミティブにより、チェーンビルダーは、一般的なトークン保有者の投票に加え、特別な管理権限を持つチェーン上の集合体を含む、高度なガバナンスシステムを構築することができます。 Substrateは、抽象的な意思決定機能に加えて、チェーン自体をアップグレードするという意思決定を含む、ガバナンスの意思決定の結果を自律的に実行することができます。

自律的な実行ステップは、Substrateベースのチェーンが主権を握るための基本的な要素です。 このチェーンは、ステークホルダーの意志を貫き、ハードフォークに参加するマイナーやバリデーターなどに依存するものではありません。 Polkadotでは、そのパラチェーンが完全な主権を行使し、独立してガバナンス面の管理を実行することができます。 このように、Polkadotの各パラチェーンやリレーチェーン自体が、それぞれのステークホルダーを持つ主権的な存在であると言えます。

Acalaは、一般評議会、技術評議会、サブプロトコルであるHomaとHonzonを管理する評議会など、複数のオンチェーン評議会を使用しています。 この中の、トークン保有者から完全に選出された一般評議会が、分散型のソブリン・ウェルス・ファンドを管理します。 運用はすべてオンチェーンで行われるため、トークン保有者はファンドの運用状況を完全に把握することができ、一般評議員の交代を投票で決めることができます。

# ファンドの運用

ファンド自体は、オンチェーンアカウントで表され、 このアカウントには、秘密鍵が関連付けられていません。 その代わりに、評議会とネットワークガバナンスがアカウントの資金を管理する能力を持っています。

資金は3つの方法でアカウントに入ります。 最初の2つは、AcalaのHonzonプロトコルで、Makerと同じような仕組みです。 Honzonは、ドルにペッグされたAcalaのステーブルコインであるaUSDの融資と引き換えに、いくつかの形態の担保を受け入れるマルチ担保のレンディングプラットフォームを提供します。 Makerと同じように、借り手はローンの安定性手数料を支払う必要があります。 また、Makerとは異なり、Acalaは手数料をバーンするのではなく、ソブリン・ウェルス・ファンドに預けます。

第二に、Acalaネットワークは、ローンの担保がある閾値を下回った場合、ペナルティ・フィーを取ります。 この手数料は、担保不足のレンディングを防ぐためのもので、ネットワークが担保の一部を清算する必要がある場合にのみ適用されます。 しかし、安定性料金と同様にそれはバーンされる燃やされるのではなくウェルス・ファンドに入ります。

第三に、AcalaはHomaというリキッドステーキングプロトコルも運営しています。 Homaは単独で記事を書く価値がありますが、レンディング・プラットフォームと同様にここではその概要を説明します。 Polkadotは、他のProof of Stakeネットワークと同様に、トークンをロックして認証者をバックアップし、ネットワークを保護します。 うまく機能した場合、これらのトークンはいくらかのリターンを得ることができますが、選ばれたバリデーターが不正をすれば、トークンはスラッシュされることになります。 このスキーマは、ネットワークセキュリティに非常に合致していますが、ファンドは同時期の目的を果たすことができるべきであるというAcalaのテーゼとは非常に矛盾しています。 Homaは、ユーザーがDOTを預けて自由に譲渡できるL-DOTと交換できるステークプールを作ることで、この関係性を調整しています（ただし、必ずしも1対1の比率ではありません）。 また、L-DOT保有者は、L-DOTをネットワークに返却することで、基本となるDOTに加え、プールからのステークス収入のシェアを取り戻し、さらに手数料を差し引いた金額がソブリンファンドに入ることになります。

収益の大部分は、他のプロトコルではトークンをバーンしてしまうようなソースから得ています。 多くのプロトコルでは、発行総数を減らすことでトークンの価値を高める仕組みとして、トークンをバーンしています。 しかし、トークンをバーンしても、価値は_創造_されず、既存の価値が再配分されるだけです。 その価値をコレクティブ・ファンドに移すことで、ネットワークはそのファンドを使って価値創造の関係を推進します。

# 価値の創造

このファンドを作っただけでもすごいことなんです。 この単一のアカウントは、自分のブロックチェーン内だけでなく、他のブロックチェーンからも複数の通貨を所有します。 そして、このアカウントはコントラクトやユーザー、ビジネス、エンティティではなく、実際にはチェーン自体が所有しています。 ちょっと立ち止まって考えてみましょう。 このチェーンは、他のチェーン資産をユーザーやコントラクトに割り当てたものではなく、あるブロックチェーン（この場合はAcala）が別のブロックチェーンにステークするものです。

通貨やトークンには様々な目的があり、Acalaのステークホルダーが資金の使い道を決めることになります。 Acalaはまず、この資金を使ってパラチェーンスロットを確保する予定です。 Polkadot has a limited number of parachain slots, and when a new one becomes available, an auction where teams bid to lock DOT determines who can use it. Most teams won’t have enough DOT on their own to secure a slot and will resort to crowdfunding by asking users to lock their DOT on behalf of the project. Acala will do the same for its first parachain auction.

But crowdfunding the same project over multiple auctions is not sustainable. If the sovereign wealth fund can raise enough funds, the blockchain itself could secure its own parachain slot and return all previous crowdfunded DOT to the contributors.

When tokens enter this fund, Acala plans to convert them all to DOT and stake it behind validators in order to grow the fund from its three revenue streams by adding staking return on DOT. When its first parachain slot is up for its renewal auction, it will unstake the DOT and use it in its own crowdfunding. Eventually, it will have enough DOT to cover the parachain bond without resorting to crowdfunding.

After Acala has its own parachain slot, it can continue the sovereign wealth fund in pursuit of other utility. Rather than accumulating DOT for the singular goal of obtaining a parachain slot, it can take positions in other parachains for access to their services or partnerships.

The effects of blockchain sovereignty extend well beyond a chain’s own governance. By combining new advances in blockchain governance, interoperability, and economics, Acala has created an innovative and sustainable funding model for their future that puts the stakeholders in control of the chain’s destiny.

# Looking Ahead

Through the dSWF and governance, Acala will become an economic and political (decision making and execution) sovereign entity. It will pioneer a new way of DAO — DAO 3.0. Just like Norway’s Sovereign Wealth Fund, Acala’s dSWF will reinvest its network surplus in foreign assets — starting with DOT and KSM and gradually diversify into other assets, for the purpose of gaining access to network security, long term wealth generation, and strategically holding stakes in valuable sovereign networks. ACA holders not only collectively own the dSWF, but also can collectively decide how to deploy the dSWF. The funds in the dSWF are essentially the Assets Under Management (AUM) of the Acala network. You can fork the code, the liquidity, and even the community, but you cannot fork AUM.

More details in the [dSWF Whitepaper](https://github.com/AcalaNetwork/Acala-white-paper/blob/master/Building_a_Decentralized_Sovereign_Wealth_Fund.pdf).

# Join Us

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launch, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot, making fast and easy to use financial applications available to everyone. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.
