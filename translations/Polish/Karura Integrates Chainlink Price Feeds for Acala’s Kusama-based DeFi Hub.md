# Karura integruje kanały cenowe Chainlink dla Centrum DeFi Acali w Kusamie

![](https://miro.medium.com/max/3200/0*dLjToIk5T5F_dSSc)

Jesteśmy podekscytowani, że [Karura](https://acala.network/karura), parachain DeFi zbudowany w sieci Kusama przez Fundację Acala, zintegrował [kanał cenowy Chainlink](https://data.chain.link/). Zdecentralizowane wyrocznie cenowe Chainlink zapewniają deweloperom inteligentnych kontraktów Karura odporne na manipulacje, hiper-niezawodne i precyzyjne dane z rynków finansowych bezpośrednio w sieci "on-chain". Deweloperzy mogą korzystać z tych danych do tworzenia bezpiecznych aplikacji i produktów DeFi mających wiele zastosowań, takich jak instrumenty pochodne, kredyty, stablecoin`y, zarządzanie aktywami i wiele innych.

Integracja ta była możliwa dzięki ostatnio uruchomionej [ Chainlink oracle pallet ](https://polkadot.network/chainlink-makes-oracle-pallet-available-to-all-substrate-polkadot-and-kusama-chains-2/), która zapewnia wystandaryzowany sposób natywnej integracji z wyrocznią Chainlink dla wszystkich projektów w ekosystemie Polkadot, w tym dla parachain`ów, sieci zbudowanych na Substrate, oraz parachain`ów Kusamy, takich jak Karura. Dzięki już gotowym kanałom cenowym Chainlink, odpornym na manipulacje (np. w celu ochrony przed atakami pożyczek błyskawicznych "flash loan") i aktywnym zabezpieczaniu wartości miliardów dolarów w całym DeFi, uważamy, że programiści Karura odniosą duże korzyści z integracji jako rozwiązania wyroczni cenowej. Nie tylko otrzymają sprawdzone zabezpieczenia Oracle i najwyższą jakość danych, ale także zaoszczędzą znaczną ilość czasu i zasobów oraz unikną ryzyka związanego z próbą wprowadzenia własnej wyroczni.

![](https://miro.medium.com/max/3200/0*ePOoL-jngB4LHFHH)

# Zabezpieczenie ekosystemu Karura za pomocą Chainlink Oracles

Jako siostrzana sieć [Acali](https://acala.network/) — centrum DeFi ekosystemu Polkadot — Karura dąży do osiągnięcia tego samego celu w ekosystemie Kusama. Kusama jest znana jako szybszy, bardziej dziki kuzyn Polkadot - sieć złożona z wielu łańcuchów, która jest zbudowana niemal identycznie, ale działa jako niezależna, samodzielna sieć z szybszymi parametrami zarządzania i wyższą tolerancją na ryzyko. Jako skalowalna, kompatybilna z EVM sieć zoptymalizowana do obsługi aplikacji DeFi, Karura pozwala Acala Foundation i niezależnym programistom przesuwać granice tego, co jest możliwe, służąc jako środowisko do wprowadzania nowych, śmiałych innowacji finansowych.

Wykorzystując zabezpieczenia typu plug-and-play Kusamy, dużą szybkość przetwarzania, mikro opłaty za gaz i interoperacyjność w różnych sieci, Karura zapewni szeroki pakiet aplikacji finansowych, w tym produkty pochodne stakowania nie wymagające zaufania (płynny KSM), wielozabezpieczony stablecoin wspierany przez aktywa międzyłańcuchowe (kUSD) oraz zdecentralizowaną wymianę przy użyciu modelu płynności AMM i mostu sieci głównej Ethereum. Aplikacje te już są zbudowane i są gotowe do uruchomienia na Kusamie, jak tylko aukcje na miejsce "slot" parachain`a zostaną uruchomione i Karura wygra miejsce. [Pobierz tokeny testnetowe](https://wiki.acala.network/learn/get-started) i wypróbuj aplikacje już dziś na [apps.acala.network](http://apps.acala.network).

![](https://miro.medium.com/max/4432/1*B8O-auSn_w1l5IgGSwhZRg.png)

Podobnie jak w przypadku każdej innej sieci blockchain lub parachain, Karura wymaga bezpiecznego, niezawodnego i dokładnego źródła danych zewnętrznych, aby umożliwić dApps reagowanie w sieci na rzeczywiste wydarzenia zachodzące poza siecią, takie jak zmiany cen aktywów. Te dane nie są natywnie generowane w sieciach blockchain i dlatego wymagają [ wyroczni cenowych sieci - blockchain oracle ](https://blog.chain.link/what-is-the-blockchain-oracle-problem/) w celu pobrania, zweryfikowania i dostarczenia do sieci. Co ważne, mechanizm wyroczni musi spełniać te same wysokie standardy bezpieczeństwa, co podstawowa sieć blockchain, aby zapobiec scenariuszowi „wejście śmieci, wyjście śmieci” z inteligentnego kontraktu.

Wybraliśmy Chainlink, ponieważ jest to najbardziej sprawdzone i solidne rozwiązanie Oracle na rynku. Programiści korzystający z Chainlink Price Feeds do tworzenia aplikacji DeFi otrzymają solidne gwarancje co do bezpieczeństwa funduszy użytkowników, a także skorzystają z rosnących efektów sieciowych Chainlink. Niektóre z nich obejmują następujące elementy:

- **Obszerny zasięg rynku** — Każdy kanał cenowy Chainlink pozyskuje dane od wielu profesjonalnych agregatorów danych, takich jak BraveNewCoin i Kaiko, którzy mają silną motywację do utrzymywania wysokiej sprawności i jakości danych. Każdy dostawca danych generuje kanały cenowe dostosowane do wolumenu, które odzwierciedlają wszystkie środowiska transakcyjne, w tym zarówno CEX, jak i DEX, dzięki czemu ich dane są precyzyjne, ale odporne na wymiany lub zgłaszanie przez dostawców danych niedokładności, przestojów lub manipulacji.
- ** Zdecentralizowana infrastruktura Oracle ** - Chainlink Price Feeds są zabezpieczone zdecentralizowanymi sieciami Oracle, składającymi się z wielu niezależnych, sprawdzonych pod względem bezpieczeństwa operatorów węzłów, prowadzonych przez wiodące narzędzia DevOps, dostawców danych i przedsiębiorstwa. Operatorzy węzłów Chainlink zapewniają wysoki poziom odporności na Sybil i mają bogate historyczne doświadczenie w aktualizowaniu kanałów cenowych nawet podczas ekstremalnych wahań rynkowych.
- ** Ekonomia skali ** - Szerokie przyjęcie i wspólne finansowanie kanałów cenowych Chainlink w ekosystemach DeFi w wielu łańcuchach generuje efekt skali, w którym projekty mogą uzyskać najlepsze dane i solidne zabezpieczenia Oracle za ułamek całkowitego kosztu. Daje również pewność, że te sieci wyroczni będą działać długoterminowo, zmniejszając przyszłe koszty przełączania lub nieoczekiwane zamknięcia.

Dzięki znormalizowanej palecie nośników Chainlink oracle, programiści Karura nie tylko mają łatwe do zintegrowania rozwiązanie cenowe, ale także otrzymują silne gwarancje, że ich aplikacja będzie działać dokładnie tak, jak napisano. Ponadto mogą albo dzielić się kosztami istniejących kanałów cenowych, albo uruchamiać nowe w oparciu o już ustalone ramy. Tak czy inaczej, nie możemy się doczekać, aby zobaczyć, co twórcy aplikacji DeFi zaczną tworzyć, łącząc Karurę i Chainlink.

[Pobierz tokeny testnetowe](https://wiki.acala.network/learn/get-started) i wypróbuj aplikacje Karura i Acala już dziś na [apps.acala.network](http://apps.acala.network).

![](https://miro.medium.com/max/2402/1\*wnveYi3ZaxxGNedEB87ZsQ.png)

## **** Informacje o Chainlink ****

Chainlink to najpowszechniej stosowany i bezpieczny sposób zasilania uniwersalnie połączonych inteligentnych kontraktów. Dzięki Chainlink programiści mogą łączyć dowolny łańcuch bloków z wysokiej jakości źródłami danych z innych łańcuchów bloków, a także danymi ze świata rzeczywistego. Zarządzany przez globalną, zdecentralizowaną społeczność setek tysięcy ludzi, Chainlink wprowadza bardziej sprawiedliwy model umów. Jego sieć zabezpiecza obecnie miliardy dolarów na inteligentne kontrakty, między innymi w zdecentralizowanych finansach (DeFi), ubezpieczeniach i ekosystemach gier.

Chainlink cieszy się zaufaniem setek organizacji, ponieważ dostarcza ostateczną prawdę za pośrednictwem bezpiecznych i niezawodnych źródeł danych. Aby dowiedzieć się więcej, odwiedź \[chain.link\] (https://chain.link/), zapisz się do \[biuletynu Chainlink\] (https://chn.lk/newsletter) i śledź \[@chainlink\] (http: / /www.twitter.com/chainlink) na Twitterze.

[Dokumenty](https://docs.chain.link/docs/getting-started) | \[] (https://www.reddit.com/r/Chainlink/) [Discord\] (https://discordapp.com/invite/aSK4zew) | \[Reddit\] (https://www.reddit.com/r/Chainlink/) | [YouTube](https://www.youtube.com/channel/UCnjkrlqaWEBSnKZQ71gdyFA) | [Telegram](https://t.me/chainlinkofficial) | \[Wydarzenia\] (https://blog.chain.link/tag/events/) | [GitHub](https://github.com/smartcontractkit/chainlink) | \[Cena\] (https://feeds.chain.link/)

## O Karura

\[Karura\] (http://acala.network/karura) to kompleksowe centrum DeFi w sieci Kusama. Założona przez fundację Acala, Karura to skalowalna, kompatybilna z EVM sieć dostosowana pod kątem DeFi. Platforma oferuje zestaw narzędzi finansowych, w tym: bezpieczną pochodną staking`u (płynny KSM), stablecoin z rozwiązaniami zabezpieczającymi, zabezpieczony przez międzyłańcuchowe aktywa (kUSD) oraz AMM DEX - wszystko z mikro opłatami za gaz, które można uiścić wsparcie tokenem.

\[Linktree\] (http://linktr.ee/karuranetwork) | \[Discord\] (https://discord.gg/vdbFVCH) | \[Strona internetowa\] (http://acala.network/karura) (** nowa **) | \[Twitter\] (https://twitter.com/KaruraNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | \[Newsletter\] (https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) | \[YouTube\] (http://youtube.com/c/acalanetwork)

## O Acala

[ Acala ](http://acala.network/) do zdecentralizowanego centrum i stablecoin na Polkadot, szybkie i górne lub aplikacje aplikacji, poprawiające efektywność handlu i finansowe czas. Platforma oferuje zestaw narzędzi finansowych: stabilizację monet z zabezpieczeniami w walorach wielu sieci, takich jak bitcoin, nie wymaga posiadania indeksu giełdowego, oraz zcentralizowaną giełdę, służenie sfinansowaniu i wspomaganiu innowacji. W istocie, Acala jest otwartą platformą narzędziową narzędzi finansowych przydatnych z inteligentnych kontraktów lub wbudowanych protokołów z gotowymi funkcjami cross-chain i solidnymi zabezpieczeniami.

[Linktree](https://linktr.ee/acalanetwork) | [Discord](https://discord.gg/vdbFVCH) | \[Strona internetowa\] (https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | \[GitHub\] (https://github.com/AcalaNetwork/Acala) | \[Wiki\] (https://github.com/AcalaNetwork/Acala/wiki) | \[Newsletter\] (https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) | \[YouTube\] (http://youtube.com/c/acalanetwork)
