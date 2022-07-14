# Acala startet den 1. Parachain im Polkadot Testnet

![Bild für Beitrag](https://miro.medium.com/max/8000/1*IGXwgFXEA7viM8upZgcw2g.jpeg)

Wir haben einen wichtigen Meilenstein auf dem Weg zur Einführung von Acala als Parachain auf Polkadot erreicht - wir haben Acala Mandala PC1 (Parachain Candidate 1) als erste Parachain auf [Rococo - Polkadots Parachain-Testnetz](https://medium.com/polkadot-network/introducing-rococo-polkadots-parachain-testnet-e3e67fc40b56) gestartet.

Rococo ermöglicht den Parachain-Konsens und die gemeinsame Sicherheit über [Cumulus](https://wiki.polkadot.network/docs/en/build-cumulus) sowie die kettenübergreifende Kommunikation über HRMP (Horizontal Relay-chain Message Passing). HRMP setzt voraus, dass kettenübergreifende Nachrichten über Relaisketten weitergeleitet werden, als Vorstufe zur späteren direkten Kommunikation von Fallschirm zu Fall über [XCMP](https://wiki.polkadot.network/docs/en/learn-crosschain) (Cross-Chain Message Passing).

Mit Acala Mandala PC1 können wir

- **Testen Sie Acalas vollständige DeFi-Suite** (Stablecoin, Staking-Derivat und DeX) unter Verwendung von kettenübergreifendem Konsens und Nachrichtenübermittlung.
- Weiterentwicklung der Implementierung des [Cross-Consensus Message (XCM)-Formats](https://github.com/paritytech/xcm-format) und insbesondere Ausarbeitung des **Cross-Chain Fungible Token-Standards**, dessen Entwicklung wir vorangetrieben haben. Der Normentwurf [hier](https://github.com/w3f/PSPs/blob/master/PSPs/drafts/psp-3.md) & PoC-Palettenimplementierung [hier](https://github.com/open-web3-stack/open-runtime-module-library/tree/rococo/xtokens).
- **Test der Acala Collator-Knoten** und Einführung von Belohnungssystemen.
- **Testen Sie kettenübergreifende Integrationen** **mit anderen Parachains** wie Laminar, Plasm, Interlay und anderen.
- Implementierung der **vertrauenslosen Absteckbrücke des Homa-Protokolls in die Relaiskette**.

# Parachain Entwicklergemeinschaft

Wir haben die folgenden Informationen an die Parachain-Entwicklergemeinschaft weitergegeben

- **Umwandlung einer substratbasierten Kette in eine Parakette** einschließlich der Umwandlung von Knoten in [Kollatoren](https://wiki.polkadot.network/docs/en/maintain-collator) durch Integration von Cumulus [hier](https://github.com/AcalaNetwork/Acala/pull/362)
- **Kettenübergreifende fungible Multi-Token-Transfer-Implementierung** - die 'xtoken'-Palette [hier](https://github.com/open-web3-stack/open-runtime-module-library/tree/rococo/xtokens). Dies ermöglicht bereits die Übertragung von ROC (Rococos Netzwerk-Token) zwischen Rococo und Mandala PC1; andere Fallschirme, die dies übernehmen oder die gleichen Standards verwenden, können Token untereinander übertragen.

# Was kommt als Nächstes

Der Mandala PC1 wird mehrmals unangekündigt zurückgesetzt, um mit der neuesten Version von Rococo Schritt zu halten, neue Funktionen einzuführen und Integrationen mit anderen Parachains zu unterstützen. Die wichtigsten bevorstehenden Entwicklungen für den Mandala Parachain-Kandidaten sind:

- **Weiterentwicklung der XCM-Palette** zusammen mit Parity, der Web3 Foundation und anderen in der Gemeinschaft bis zur Produktionsreife.
- **Acala-Stacking** mit Belohnungen/Slash auf Acala Collator-Knoten aktivieren.
- **Ausführliches Testen der kettenübergreifenden Kommunikation** mit anderen Parachains und Ermöglichung einiger Anwendungsfälle, die isoliert implementiert wurden, z. B. Kreuzung von aUSD mit Laminar als Basiswährung für den Margin-Handel und Kreuzung von aUSD mit dem Plasm-Netzwerk als Zahlungsmittel.
- **Enable Homa Staking Derivative (LDOT) Relay-Chain Bridge**, so dass die vertrauenswürdige flüssige Absteckung für Kusama und Polkadot beim Start bereit ist.

# Launch

Neben Rococo und Mandala wird Acala sein kanarisches Netzwerk Karura als Parachain zunächst auf Kusama starten, wenn die Parachain-Funktion dort aktiviert ist, und dann das Hauptnetz auf Polkadot. Acala wird die beiden Netzwerke - Karura & Acala mainnet - betreiben, um DeFi-Infrastruktur und Liquidität für das Kusama- und Polkadot-Ökosystem bereitzustellen. Von nun an werden wir uns auf die Parachain-Auktion vorbereiten, um uns einen Sendeplatz zu sichern und in den beiden Netzen zu starten. **Abonniere** [**hier**](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) **um aktuelle Informationen über die Versteigerung und den Start von Acala parachain zu erhalten.**

# Über Acala

[Acala](http://acala.network/) ist das erste dezentralisierte Finanzkonsortium seiner Art mit der Vision, finanzielle Stabilität, Liquidität und Zugänglichkeit in den Mainstream zu bringen. Das Acala-Netzwerk ist ein kettenübergreifendes Finanzzentrum für das Polkadot-Ökosystem und darüber hinaus. Es bietet eine Reihe von Finanzprimitiven: einen mehrfach besicherten Stablecoin, der durch kettenübergreifende Vermögenswerte wie Bitcoin abgesichert ist, ein vertrauensloses Staking-Derivat und eine dezentrale Börse, um Liquidität freizusetzen und finanzielle Innovationen voranzutreiben. Sie ist die erste offene Plattform für finanzorientierte dApps, die mit Smart Contracts oder integrierten Protokollen mit sofortigen Cross-Chain-Fähigkeiten, Sicherheit und finanziellen Optimierungen bereitgestellt werden.

**Beitreten**

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

![Bild für Beitrag](https://miro.medium.com/max/1500/0*YTeYSsHAVjOBCZu8.jpeg)

Acala ist ein stolzer Stipendiat der Web3 Foundation
