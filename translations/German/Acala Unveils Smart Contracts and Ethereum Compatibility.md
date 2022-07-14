# Acala stellt Smart Contracts und Ethereum-Kompatibilität für Polkadot DeFi vor

## Acala unterstützt jetzt das EVM und Tinte! Paletten auf Substrate, die Solidity- und Wasm-basierte Smart Contracts für Entwickler ermöglichen

![Bild für Beitrag](https://miro.medium.com/max/1600/0*-4rCl6SjqDKz7eBh)

Von [Acala Network](https://medium.com/u/241f963260c9?source=post_page-----588b3891e53d--------------------------------)

Polkadot ist sowohl für die einfache Integration mit anderen Blockchains wie Bitcoin und Ethereum (über Bridges wie Interlay und RenVM) als auch für den Betrieb einer Reihe heterogener (aka unabhängiger und anpassbarer), aber miteinander verbundener Chains, genannt Parachains, ausgelegt. Polkadot ist mehr wie eine Layer-0-Infrastrukturkette, die die zugrunde liegende Vertrauensschicht bereitstellt, die mit gemeinsamer Proof of Stake (PoS)-Sicherheit und Cross-Chain-Kommunikation einhergeht. Die Parachain-Ketten sind eher domänenspezifische Ketten, die für ihre Anwendungsfälle optimiert sind und spezifische Domänenprobleme lösen, wobei Acala die Domäne der dezentralen Finanzen besetzt. Wir bieten eine Reihe von sofort einsatzbereiten DeFi-Primitiven wie einen Stablecoin (aUSD), Staking-Derivate (z. B. die Möglichkeit, Token (LDOT) gegen gestackte/gesperrte DOT einzulösen) und eine dezentrale Börse, um weitere DeFi-Innovationen voranzutreiben. Wir haben auch allgemeine Utility-Module wie ein Orakel, mehrere Währungen und ein generisches Überwachungs-Framework für Teams zur Verfügung gestellt.

Substrat-basierte Parachains wie Acala werden den kompletten Tech-Stack genießen, der von diesem Framework bereitgestellt wird - von der technischen Infrastruktur auf niedriger Ebene (RPC, Web-Assembly-Laufzeit, Peer-2-Peer-Kommunikation usw.) bis hin zu Modulen auf der Anwendungsebene, die EVM (Ethereum Virtual Machine) und Smart Contract-Funktionen ermöglichen. Das bedeutet, dass in absehbarer Zukunft Innovationen und technologische Weiterentwicklungen auf Kettenebene in einer noch nie dagewesenen Geschwindigkeit und in großem Umfang stattfinden werden; neue Funktionen werden durch Plug-and-Play über forkless Upgrades in allen Substrat-basierten Ketten einfach und nahtlos verfügbar sein (siehe Beispiele auf [Substrat-Marktplatz](https://marketplace-staging.substrate.dev/)).

Dies vorausgeschickt, hat Acala nun Smart Contract-Fähigkeiten auf folgende Art und Weise aktiviert:

1.  Acala unterstützt die EVM-Palette (auch bekannt als Laufzeitmodul), die im Wesentlichen eine Ethereum Virtual Machine-Implementierung auf Substrate ist, so dass Solidity-Verträge auf Acala bereitgestellt und ausgeführt werden können.
2.  Acala unterstützt auch die Tinte! Vertragspalette, die Wasm (Web Assembly) basierte substratnative Smart Contracts ermöglicht, die in Rust geschrieben sind.

Dieses Update wird sowohl durch den technischen Fortschritt als auch durch die Interessen der Community vorangetrieben. Acala unterstützt eine Reihe von Protokollen bei der Erforschung von kettenübergreifenden DeFi-Einsätzen auf Polkadot, deren Mechanismen wir in diesem Artikel auspacken werden, und Smart Contracts ist sicherlich einer der wichtigen Wege, die es zu erforschen gilt. Im Folgenden wird Acala aktiver mit [Parity](https://www.parity.io/) und anderen im Ökosystem wie [Moonbeam](https://moonbeam.network/), [Plasm](https://www.plasmnet.io/) und [Edgeware](https://edgewa.re/) zusammenarbeiten und zur Entwicklung von EVM und Smart Contracts beitragen.

# Wir gehen nun auf die folgenden Themen ein:

1.  Cross-Chain-Liquidität über Brücken
2.  Wege auf Polkadot zu setzen
3.  Wege auf Kusama zu setzen
4.  Wege auf Acala zu setzen
5.  Der aktuelle Stand der Smart Contracts auf Polkadot

# Cross-Chain-Liquidität über Brücken

Bridges sind interoperable Technologien, um Assets und Nachrichten zwischen zwei wirtschaftlich souveränen und technologisch unterschiedlichen Chains zu übertragen, z.B. zwischen Polkadot und Ethereum oder Bitcoin. Es gibt verschiedene Varianten von Bridges, von zentralisiert und vertrauenswürdig bis hin zu eher dezentralisiert und vertrauenslos.

1.  **Vertrauenslösungen**: Sie verwenden Multi-Sig- oder Proof of Authority (PoA)-Aufbauarten, sie sind relativ einfach zu implementieren und können bereits jetzt verwendet werden. [ChainX](https://chainx.org/) als Bitcoin-Brücke und [ChainSafe](https://chainsafe.io/) als Ethereum-Brücke sind Beispiele für diesen Typ, mit Roadmaps, um mit der Zeit dezentraler zu werden.
2.  **Vertrauenslose Lösungen**: Verwendung von wirtschaftlichen und/oder kryptographischen Garantien, um Vermögenswerte zu/von zwei Blockchains zu übertragen; sie sind vertrauenslos, könnten aber für die Benutzer teuer sein und befinden sich außerdem aufgrund der technischen Herausforderungen ihrer vertrauenslosen Natur noch in der Forschung und Entwicklung. [Interlay](https://medium.com/interlay/bitcoin-on-polkadot-proof-of-concept-for-trustless-bridge-shipped-6fb8e549bef0) als Bitcoin-Brücke und [SnowFork](http://www.snowfork.com/) und [Darwinia](https://darwinia.network/) als Ethereum-Brücke sind Beispiele für diesen Typ.
3.  **Hybrid Custodial/Trustless Lösungen**: dann gibt es die [RenVM](https://renproject.io/) Lösung, die permissionless ist mit großartiger UX und Popularität mit einem klaren Weg in Richtung Dezentralisierung, aber im Moment wird viel Vertrauen in das Ren-Team gesetzt.

Acala ist neutral in Bezug auf Lösungsansätze für Brücken, da verschiedene Arten von Brücken unterschiedliche Benutzerpräferenzen in Bezug auf Vertrauenswürdigkeit, Bequemlichkeit und Kosten befriedigen können und es gute Gründe dafür gibt, dass verschiedene Arten von Brücken nebeneinander existieren und verschiedene Bedürfnisse bedienen.

# Einsatz auf der Polkadot Relais Kette

Wie bereits erwähnt, handelt es sich bei Polkadot um eine kettenübergreifende Layer-0-Infrastrukturkette (genannt [Relay Chain](https://wiki.polkadot.network/docs/en/learn-architecture#relay-chain)). Anwendungen und Protokolle können daher nicht direkt auf der Relaiskette eingesetzt werden, sondern über die folgenden Mechanismen, die als Bestandteile des Polkadot-Netzwerks bereitgestellt werden, jeweils mit ihren eigenen Kompromissen:

1.  **Einsatz als Parachain** - Diese Option hat den höchsten Grad an Anpassbarkeit und Flexibilität, sowohl technisch als auch wirtschaftlich. Es hat einen "dauerhafteren" Zugang (innerhalb der Parachain-Mietdauer) zur gemeinsamen Sicherheits- und Cross-Chain-Kommunikationseinrichtung von Polkadot. Die Einrichtung ist jedoch mit höheren Kosten verbunden und erfordert viel mehr Aufwand für den Aufbau und die Pflege des Netzwerks sowie der Community. Sie können einen Vorgeschmack darauf bekommen, indem Sie [Acala](https://github.com/AcalaNetwork/Acala/wiki/1.-Get-Started) erforschen.
2.  **Einsatz als Parathread** - ist technisch ähnlich wie Parachain, verwendet aber ein Pay-as-you-go-Modell für Sicherheit und Kommunikationszugang, daher weniger Aufwand im Vorfeld und billiger im Betrieb. Wenn eine Kette keinen Parachain-Slot bekommen kann, kann sie auf Parathread zurückgreifen, um ihre Operationen fortzusetzen.
3.  **Einsatz als DApp auf einer aktiven Parachain/Parathread** - für Teams, die auf das Polkadot-Ökosystem zugreifen wollen, aber keine Blockchain aufbauen und pflegen wollen, oder die Dinge ohne große Vorabverpflichtung ausprobieren wollen, könnte der Einsatz auf einer bestehenden Parachain eine gute Option sein. Besonders für DeFi bezogene DApps können Sie Acala als Landeplatz (wie in [Rens Fall](https://medium.com/acalanetwork/bringing-btc-to-polkadot-acala-x-ren-e7959855d5aa?source=collection_home---4------6-----------------------).) und als technisch versierten Polkadot-Buddy bei der Erkundung des Raums behandeln.

Neben technischen und wirtschaftlichen Überlegungen ist auch an die Zusammensetzbarkeit zu denken. Der Grad und die Raffinesse der Zusammensetzbarkeit kann variieren, je nachdem, wo Sie landen - DApps auf einer Parachain würden natürlich einen höheren Grad an Zusammensetzbarkeit innerhalb dieser Kette genießen (lesen Sie Rens Integration [hier](https://github.com/AcalaNetwork/Acala/wiki/T.-Cross-chain-DeFi#ren)), parachain-übergreifende DApps können eine geringere Zusammensetzbarkeit und Atomizität der Transaktionen haben (lesen Sie Laminars Integration [hier](https://github.com/AcalaNetwork/Acala/wiki/T.-Cross-chain-DeFi#laminar)), und Bridges können eine noch geringere Zusammensetzbarkeit haben, da sie sich hauptsächlich auf Werttransfers und bestimmte spezifische Nachrichtenübermittlung über bestimmte Blockchains konzentrieren.

# Einsatz in Kusamas Relaiskette

[Kusama](http://kusama.network), ähnlich wie Polkadot, ist eine kettenübergreifende Layer-0-Infrastrukturkette mit einer Kern-[Relais-Kette](https://wiki.polkadot.network/docs/en/learn-architecture#relay-chain), die Sicherheit und Interoperabilität bietet. Kusama ist als Entwicklungsumgebung für Teams gedacht, die sich auf den Einsatz auf Polkadot vorbereiten, oder für Teams, die ausschließlich auf Kusama bauen wollen, um niedrigere wirtschaftliche Barrieren für Parachain-Slots und schnellere Governance-Zyklen zu erreichen. Entwickler haben mit Kusama die gleichen Möglichkeiten wie mit Polkadot, mit ein paar Einschränkungen:

1.  **Einsatz als Parachain** - Teams können eine Parachain auf Kusama aus drei Hauptgründen aufbauen. Zunächst können die Fallschirme nach bestandenen Tests im Westend-Testnetz auf Kusama eingesetzt werden, um ihre Technologie vor einem vollständigen Einsatz auf Polkadot fein abzustimmen. Einige Teams, darunter auch Acala, werden sich dafür entscheiden, sowohl auf Polkadot als auch auf Kusama Parachains zu betreiben, um beide Gemeinden zu bedienen. Drittens können sich Teams (z.B. neue Startups) auch dafür entscheiden, ausschließlich auf Kusama zu bleiben, wenn die Kosten für einen Polkadot-Parachain-Slot unerschwinglich sind oder wenn sie die Risikobereitschaft und Schnelllebigkeit von Kusama bevorzugen. Die Kusama-Parachain-Option ist ebenfalls anpassbar und flexibel, sowohl technisch als auch wirtschaftlich.
2.  **Einsatz als Parathread** - Kusama wird die gleiche Parathread-Funktionalität wie Polkadot haben, was ein Pay-as-you-go-Modell für Sicherheit und Kommunikationszugang ist, was zu weniger Overhead und Kosten beim Betrieb führt. Ein Kompromiss ist, dass Parathreads mit weniger häufigen Blockübertragungen an die Relay Chain einhergehen, so dass sie für einige Anwendungsfälle besser geeignet sind als für andere.
3.  **Einsatz als DApp auf einer aktiven Parachain/Parathread** - DApps können auf Kusama-Parachains oder Parathreads aufgebaut werden. DeFi DApps zum Beispiel können auf Acalas Kusama Network aufgebaut werden, ebenso wie viele andere Anwendungsfälle wie Gaming, Kommunikation, soziale Medien oder DAOs.

Im nächsten Abschnitt werden wir verschiedene Möglichkeiten für den Einsatz auf Acala parachain untersuchen.

# Deployment auf dem Acala Fallschirm

Sie können Acala als DeFi-Landeplatz für Polkadot und Kusama und als Ihren technisch versierten Builder-Buddy behandeln. Es gibt derzeit drei Möglichkeiten, wie Sie auf Acala bereitstellen können:

1.  **Laufzeitmodule (auch Paletten genannt)** - dies ermöglicht die höchste Stufe der Anpassbarkeit und den Zugriff auf die Kettenlogik von Acala für eine anspruchsvollere Integration. Es verfügt nicht über die ausfallsichere Sandbox-Umgebung, die Smart Contracts genießen, daher erfordert es Sicherheits-Audits und bedarf der Genehmigung durch die Governance. Es eignet sich besser für Infrastruktur- und Allgemeingut-Protokolle. Das [RenVM-Brückenmodul](https://github.com/AcalaNetwork/Acala/tree/master/ecosystem-modules/ren/renvm-bridge) ist ein gutes Beispiel dafür. Ein brandneues Konto mit nur frisch geprägten renBTC, kann beliebige Transaktionen auf Acala durchführen, ohne einen Gebühren-Token zu benötigen. Dank der FlexFee-Funktion von Acala sind Token wie renBTC neben ACA, aUSD und DOT als einer der Standard-Gebühren-Token nativ integriert.
2.  **Solidity-Smart-Verträge bereitstellen** - für diejenigen, die einen Teil oder alle ihre bestehenden Solidity-Smart-Verträge zu Polkadot migrieren möchten, ohne den gesamten Code neu zu schreiben, kann dies ein guter Ausgangspunkt sein. Als Beispiel würden einige Teams eine Bridge verwenden, um ihre Token von Ethereum zu Polkadot zu übertragen und dann auf Acala einzusetzen, um schnellere und günstigere Transaktionen und eine bessere Benutzererfahrung zu erhalten.
3.  **Tinte ausgeben! Smart Contracts** - dies ist Substrates nativer, Rust-basierter Wasm Smart Contract, lesen Sie mehr darüber, wie er mit EVM verglichen wird [hier](https://substrate.dev/docs/en/knowledgebase/smart-contracts/ink-fundamentals).

Die Smart-Contract-Module stehen kurz vor der Produktionsreife, sind aber noch nicht (nach Acala-Standard) produktionsreif. Wir werden eng mit Parity und anderen im Ökosystem zusammenarbeiten, um sie fertigzustellen. Wir skizzieren die Vorbehalte und den aktuellen Stand der Entwicklung im nächsten Abschnitt.

# Der aktuelle Stand von Smart Contracts

## EVM

Während Solidity- und EVM-kompatible Verträge auf Substrate-basierten Ketten wie Acala eingesetzt und ausgeführt werden können, wird ein Großteil des Toolings noch entwickelt, damit es mit bestehenden Entwicklungswerkzeugen wie Truffle und Remix etc. kompatibel ist. SDKs werden auch entwickelt, um mit bestehenden web3.js und anderen Bibliotheken kompatibel zu sein. Acala wird sich auch auf die Verbesserung der Zusammensetzbarkeit von Smart Contracts und Laufzeitmodulen konzentrieren, um kettenübergreifende DeFi-Innovationen zu beschleunigen.

## Tinte! Smart Contracts

Rostbasierte Tinte! Smart-Contract-Sprache befindet sich noch in der Entwicklung, ebenso wie die dazugehörigen Entwicklungswerkzeuge (cargo-contract und [Redspot](https://github.com/patractlabs/redspot) - Truffle für Ink!) und SDKs (polkadot.js).

# Nächste Schritte

Acala unterstützt jetzt EVM mit der [Frontier](https://github.com/paritytech/frontier) Substrate-Ethereum-Kompatibilitätsschicht. Wir können jetzt unmodifizierte Ethereum DApps ausführen. Als nächstes werden wir komplexere (reale) Solidity-Verträge implementieren, Tooling-Unterstützung einschließlich Metamasken testen und die Integration von Paletten (Laufzeitmodulen) implementieren, um die Kompatibilität zu verbessern und mit ERC20 und anderen Token-Standards kompatibel zu werden.

Betrachten Sie dies als Ihre offizielle Einladung zu [**Build with Acala**](https://github.com/AcalaNetwork/Acala/wiki/U.-Build-with-Acala), wo wir Teams bei der Erstellung wertvoller kettenübergreifender DeFi-Projekte mit Polkadot und Kusama unterstützen und helfen.

# Beitreten

[Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

Um über die Fortschritte bei der Einführung von Acala Parachain auf Polkadot und Kusama auf dem Laufenden zu bleiben, abonnieren Sie den [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

# Über Acala

[Acala](http://acala.network/) ist der dezentrale Finanz-Hub von Polkadot, der es schnell und einfach macht, Finanzanwendungen zu nutzen oder zu erstellen, die Effizienz des Handels zu verbessern und wertvolle Zeit zu sparen. Die Plattform bietet eine Reihe von Finanzprimitiven: einen mehrfach besicherten Stablecoin, der durch kettenübergreifende Vermögenswerte wie Bitcoin gesichert ist, ein vertrauensloses Staking-Derivat und eine dezentrale Börse, um Liquidität freizusetzen und finanzielle Innovationen voranzutreiben. Acala ist die de facto offene Plattform für Finanzanwendungen zur Nutzung von Smart Contracts oder eingebauten Protokollen mit Out-of-the-Box-Cross-Chain-Fähigkeiten, Sicherheit und Finanzoptimierungen.
