# Acala Sicherheitsaudit

![Bild für Beitrag](https://miro.medium.com/max/8000/1*yhydywHe1k2421hd6xqhFQ.jpeg)

Wir bei Acala sind der Meinung, dass jeder einzelne Nutzer, nicht Unternehmen, die Kontrolle über seine Finanzen haben sollte. Unsere Aufgabe ist es, finanzielle Anwendungen des Web 3.0 zu unterstützen und zu fördern - das wirklich dezentralisierte und "vertrauenslose" Web. Eine offenere und gerechtere finanzielle Zukunft ist das, was wir mit unserer DeFi optimierten Smart Contract Plattform und unseren Protokollen - dezentraler Stablecoin, vertrauenswürdiges Liquid Staking und dezentraler Austausch - zu ermöglichen hoffen.

Die Sicherheit der Acala-Blockchain und -Protokolle hat für uns jedoch höchste Priorität. Wir haben beträchtliche Anstrengungen unternommen, um eine Plattform und die dazugehörigen Protokolle zu entwickeln, die wir für sicher und zuverlässig halten. Außerdem haben wir die Besten der Branche damit beauftragt, unsere Codebasis zu prüfen - darunter [SRLabs](https://srlabs.de/), [Trail of Bits](https://www.trailofbits.com/) und [Slow Mist](https://www.slowmist.com/en/).

![Bild für Beitrag](https://miro.medium.com/max/1730/1*hKvzkJVXDmSA9OU7NhFLuA.jpeg)

Der Umfang der Prüfung umfasste alle Laufzeitimplementierungen von Acala, einschließlich des Ökosystemmoduls RenVM, der von der Gemeinschaft gepflegten ORML-Module, von denen Acala abhängt, sowie der Front-End-Schnittstelle für die DApp von Acala. Bislang haben SRLabs und Slow Mist ihre Prüfungen abgeschlossen, und die Prüfung von Trail of Bits soll im Januar 2021 beginnen.

# Der Bericht & Fixes

Bei der Prüfung durch SRLabs wurden 0 kritische, 1 hochgradige, 7 mittlere und 2 geringgradige Probleme festgestellt.

Bei der SlowMist-Überprüfung wurden 0 kritische, 0 hohe, 1 mittleres und 1 geringfügiges Problem festgestellt.

Das eine wichtige Problem im Zusammenhang mit der Gewichtszuweisung war eine geplante Aufgabe, die zum Zeitpunkt der Prüfung noch nicht umgesetzt war. Wir haben nun das Benchmarking abgeschlossen und eine angemessene Gewichtung für alle [extrinsischen](https://substrate.dev/docs/en/knowledgebase/learn-substrate/extrinsics) (d.h. signierte/unsignierte Transaktionen und Vererbungen - Informationen, die in einem Block enthalten sind, aber nicht geklatscht werden) festgelegt.

Alle anderen Fragen der Netzsicherheit wurden von den Prüfern behandelt und überprüft. Zwei anwendungsbezogene Probleme (Nr. 5 und Nr. 8 im SRLabs-Bericht) sind allgemeine DeFi-Probleme, wie z. B. das DeX-Front-Running, für die es noch keine zufriedenstellende Lösung gibt. Wir gehen das Problem unter dem Gesichtspunkt des Risikomanagements an, indem wir sichere Parameter festlegen. Darüber hinaus streben wir weitere Wirtschaftsprüfungen an, bei denen simulationsbasierte Marktstresstests zum Einsatz kommen, damit wir Schwachstellen und Marktrisiken in einem skalierten Umfang und Wert bewerten können.

Den vollständigen Bericht von SRLabs und SlowMist finden Sie [hier](https://github.com/AcalaNetwork/Acala/tree/master/audit)

# Vorwärts bewegen

Audits sind nur ein Teil unserer Bemühungen zur Gewährleistung der Sicherheit und zum Risikomanagement. Alle Laufzeit-Codebasen von Acala werden geprüft, und bei der Entstehung werden alle Bilanzen und Governance-Entscheidungen öffentlich überprüfbar sein. Unser [Bug Bounty Programm](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#runtime-bug-bounty) ist ebenfalls ein wichtiger Bestandteil, um unsere Codebasis sicher zu halten, und wir ermutigen Entwickler, sich mit unserem Code zu beschäftigen und Schwachstellen zu melden. Wir glauben, dass Transparenz, Zeit und Wert die wahren Tests für die Sicherheit eines Netzwerks und von Protokollen sind; seien Sie also bitte wachsam und helfen Sie uns, Acala für alle sicherer zu machen.

# Beitreten

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

Um über die Fortschritte bei der Einführung von Acala parachain auf dem Laufenden zu bleiben, abonnieren Sie den [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

# Über Acala

[Acala](http://acala.network/) ist das dezentrale Finanzzentrum von Polkadot, das schnelle und einfach zu bedienende Finanzanwendungen für jedermann zugänglich macht. Die Plattform bietet eine Reihe von Finanzprimitiven: einen mehrfach besicherten Stablecoin, der durch kettenübergreifende Vermögenswerte wie Bitcoin abgesichert ist, ein vertrauensloses Staking-Derivat und eine dezentrale Börse, um Liquidität freizusetzen und Finanzinnovationen zu fördern. Acala ist die de facto offene Plattform für Finanzanwendungen zur Nutzung von Smart Contracts oder integrierten Protokollen mit sofort einsetzbaren Cross-Chain-Funktionen, Sicherheit und finanziellen Optimierungen.
