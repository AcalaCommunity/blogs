# Acala uruchamia pierwszy Parachain w Testnecie Polkadot

![Obraz do wpisu](https://miro.medium.com/max/8000/1*IGXwgFXEA7viM8upZgcw2g.jpeg)

Osiągnęliśmy znaczący postęp w kierunku wprowadzenia Acala jako parachain na Polkadot - uruchomiliśmy testnet Acala Mandala PC1 (Parachain Candidate 1) jako pierwszy parachain w [ Rococo - Polkadot parachain testnet ](https://medium.com/polkadot-network/introducing-rococo-polkadots-parachain-testnet-e3e67fc40b56).

Rococo umożliwia parachain konsensus i współdzielone bezpieczeństwo za pośrednictwem [ Cumulus ](https://wiki.polkadot.network/docs/en/build-cumulus), a także międzyłańcuchową komunikację za pośrednictwem HRMP (przekazywanie wiadomości w łańcuchu poziomym). HRMP wymaga, aby komunikaty międzyłańcuchowe były kierowane przez łańcuchy przekaźnikowe, jako krok w kierunku bezpośredniej komunikacji parachain z parachain za pośrednictwem późniejszego [ XCMP ](https://wiki.polkadot.network/docs/en/learn-crosschain) (Cross-chain Message Passing).

Dzięki Acala Mandala PC1 możemy

- ** Przetestuj pełny pakiet Acala DeFi ** (stablecoin, instrumentów pochodne staking`u i DeX) przy użyciu konsensusu międzyłańcuchowego i przekazywania wiadomości.
- Rozwiń dalej implementację [ formatu Cross-Consensus Message (XCM) ](https://github.com/paritytech/xcm-format), a konkretnie dopracuj ** krzyżowy standard zamiennego tokena **, który opracowaliśmy. Wersja robocza standardu [ tutaj ](https://github.com/w3f/PSPs/blob/master/PSPs/drafts/psp-3.md) & Implementacja palety PoC [ tutaj ](https://github.com/open-web3-stack/open-runtime-module-library/tree/rococo/xtokens).
- ** Testuj węzły Acala Collator ** i wdrażaj schematy nagród.
- ** Testuj integracje międzyłańcuchowe ** ** z innymi parachain`ami **, takimi jak Laminar, Plasm, Interlay i inne.
- Zaimplementuj protokołu Homa ** zaufany most staking`u do łańcucha zależnego **.

# Społeczność programistów Parachain

Udostępniliśmy następujące informacje społeczności programistów parachain

- ** Zamień łańcuch oparty na Substrate na parachain **, włąćzając w to zamianę węzłów w [ kolektor ](https://wiki.polkadot.network/docs/en/maintain-collator), integrując Cumulus [ tutaj ](https://github.com/AcalaNetwork/Acala/pull/362)
- ** Implementacja międzyłąńcuchowego przesyłu różnych (wielu) tokenów ** - paleta „xtoken” [ tutaj ](https://github.com/open-web3-stack/open-runtime-module-library/tree/rococo/xtokens). To już umożliwia przesyłanie ROC (token sieciowy Rococo) pomiędzy Rococo i Mandala PC1; inne parachain`y, które to przyjmą lub używają tych samych standardów, mogą przekazywać sobie tokeny.

# Co dalej

Mandala PC1 będzie wielokrotnie resetowana niezamierzenie i niezapowiedzianie, aby nadążyć za najnowszą wersją Rococo, wprowadzać nowe funkcje i wspierając integracje z innymi parachain`ami. Najważniejszymi wydarzeniami zbliżającymi się do Parachain`a Mandala są:

- ** Kontynuowanie rozwoju palety XCM, ** wraz z Parity, Fundacją Web3 oraz innymi członkami społeczności, aby była gotowa do produkcji.
- ** Uruchomienie staking`u Acala ** z nagrodami / cięciami na węzłach Acala Collator.
- ** Wyczerpujące testy komunikacji międzyłańcuchowej ** z innymi parachan`ami, umożliwiają zastosowania, które zostały wdrożone osobno, na przykład połączenie aUSD z Laminar jako walutę bazową do handlu z depozytem zabezpieczającym, czy połączenie aUSD z siecią Plasm jako metody płatności.
- ** Uruchomienie pochodnej staking`u (LDOT) Homa z mostem do łańcucha zależnego **, tak aby zaufany płynny staking dla Kusama i Polkadot był gotowe do uruchomienia.

# Uruchomienie

Poza Rococo i Mandala, Acala uruchomi swoją sieć ostrzegawczą Karura jako parachain, najpierw na Kusama, kiedy funkcja parachain będzie już włączona, a następnie uruchomieni swój mainnet na Polkadot. Acala będzie obsługiwać dwie sieci - Karura & Acala mainnet, co zapewni infrastrukturę dla DeFi i płynność dla obu ekosystemów Kusama i Polkadot. Od tego momentu będziemy przygotowywać się do aukcji parachain w celu zabezpieczenia miejsca (slot) oraz uruchomienia w obu sieciach. ** Zasubskrybuj ** [** tutaj **](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) **, aby otrzymywać informacje o aukcji parachain`u Acala i jej uruchomieniu. **

# O Acala

[ Acala ](http://acala.network/) to pierwsze w swoim rodzaju zdecentralizowane konsorcjum finansowe z wizją wprowadzenia stabilności finansowej, płynności i dostępności do głównego nurtu. Sieć Acala to międzyłańcuchowe centrum finansowe dla ekosystemu Polkadot i nie tylko. Oferuje zestaw narzędzi finansowych: stablecoin z zabezpieczeniami w wielu międzyłańcuch walorach, takich jak Bitcoin, nie wymagająca zaufania pochodna staking`u, oraz zdecentralizowana giełda, w celu zapewnienia płynności i aby napędzać innowacje finansowe. Jest to otwarta platforma dla dApps zorientowanych na finanse, którą można wdrożyć przy użyciu inteligentnych kontraktów lub wbudowanych protokołów z gotowymi funkcjami cross-chain, bezpieczeństwem i optymalizacjami finansowymi.

**Dołącz do nas**

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

![Obraz do wpisu](https://miro.medium.com/max/1500/0*YTeYSsHAVjOBCZu8.jpeg)

Acala jest dumnym stypendystą Fundacji Web3
