# Build Acala: Polkadot parachain testnet Rococo, współpraca z Ren, Mandala testnet mania, na The Defiant | Sierpień 2020

Lipiec był miesiącem budowania ze współpracownikami ekosystemu, takimi jak [ Ren ](https://renproject.io/) i [ Laminar ](http://laminar.one/), testując sieć z dziesiątkami tysięcy nowych kont i transakcji podczas kampanii sieci testowej 3. Sezonu Mandala Festival, oraz przygotowania się do uruchomienia na parachain`owej sieci testowej Polkadot Rococo.

![Image for post](https://miro.medium.com/max/8000/1*6wJEyP0ojcA8zM3SZAPzqQ.jpeg)

# **Aktualizacja programowania**

- ** Sieć testowa parachain`u na Polkadot ** [ ** Rococo: ** została uruchomiona ](https://polkadot.network/introducing-rococo-polkadots-parachain-testnet/) na początku tego tygodnia, co stanowi znaczący krok w kierunku integracji między łańcuchami. Parachain`y, aby korzystać ze wspólnych zabezpieczeń, teraz mogą łączyć się z łańcuchem sieci przekaźnikowej (od której zależą) - Relay, a także już możliwe jest bardzo oczekiwane wysyłanie wiadomości między łańcuchami, choć jest ograniczone do poziomego przesyłania wiadomości, w którym łańcuch sieci Relay będzie używany do kierowania wiadomości między dwoma parachain`ami. Acala pracuje nad rejestracją w sieci Rococo, aby przetestować funkcjonalności.
- [** Moduł mostu RenVM **](https://github.com/AcalaNetwork/Acala/tree/master/ecosystem-modules) ** & Integracja renBTC: ** została wdrożona w sieci testowej Acala Mandala TC4, stanowiąc pierwszy krok w przeniesieniu renBTC do Acali i ekosystemu Polkadot. renBTC jest teraz tokenem opłat, może służyć jako zabezpieczenie linii kredytowej dla stablecoin`ów i jest notowany na Acala DeX.
- ** Substrate RC4 **: Mandala TC4 jest teraz zaktualizowana do [ Substrate RC4 ](https://github.com/paritytech/substrate/releases/tag/v2.0.0-rc4), co umożliwia transakcje atomowe - jest to krok bliżej do gotowych do produkcji smart kontraktów i wkrótce zostanie zaktualizowana do najnowszej TC5 po zakończeniu kampanii sieci testowej.
- ** Acala Pulse **: panel analityczny służący do śledzenia statystyk sieci jest w trakcie budowy i zostanie udostępniony w przyszłym tygodniu. Użytkownicy mogą śledzić podstawy systemu - emisję aUSD, wolumen DeX i ilość DOT w płynnym staking`u, a także ryzyka systemu, likwidacje i aukcje itp.
- ** Ćwiczenie Czarnego Czwartku & Awaryjne wyłączenie **: w przyszłym tygodniu, [ w ramach Mandala Festival ](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#week-3-black-thursday-simulation), przeprowadzimy symulację zmienności Czarnego Czwartku, przetestujemy hybrydowy mechanizm likwidacji, który obejmuje DeX i aukcje, aby skutecznie odzyskać pożyczki. Następnie wprowadzimy awaryjne zamknięcie systemu, przetworzymy wszystkie niespłacone pożyczki i poprosimy użytkowników o odzyskanie zabezpieczeń z koszyka aktywów. _ Zasady 3. tygodnia festiwalu & nagrody są _ [_ tutaj _](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#week-3-black-thursday-simulation) _._

  ![Image for post](https://miro.medium.com/max/2880/1*XQbgIIFPlzwrK8L1eXdKew.jpeg)

# **Aktualizacja ekosystemu**

- [** Ren x Acala / Polkadot **](https://medium.com/acalanetwork/bringing-btc-to-polkadot-acala-x-ren-e7959855d5aa?source=collection_home---4------2-----------------------) ** aby ** wprowadzić Bitcoin, a w przyszłości inne izolowane klasy aktywów do Acali i do szerszego, wielołańcuchowego wszechświata Polkadot.
- [** Mandala Festival Season # 3 **](https://medium.com/acalanetwork/acala-mandala-festival-season-3-d0a6f155c154?source=collection_home---4------1-----------------------): rozpoczął się dwa tygodnie temu, wywołał spory szum dzięki **_ ponad 100 000 transakcji, 13 000 nowych kont, 2,5 + miliona aUSD wydanych z zabezpieczeń renBTC i ponad 250 wykopanych renBTC (sieci testowej) _**. Sprawdź [ działania w Subscan ](https://acala-testnet.subscan.io/).
- [** Hackusama z Acala **](https://medium.com/acalanetwork/hackusama-ea1ddf3e945a): Acala jest partnerem edukacyjnym dla Hackusamy, dostarczającym wszystkie swoje palety wykonawcze i [ wspólne biblioteki ](https://github.com/open-web3-stack/open-runtime-module-library), takie jak Oracle i paleta wielo-tokenowa, wsparcie techniczne i porady dla zespołów budujących projekty DeFi.
- ** Fundacja Acala jest teraz członkiem rady ** Polkadot aktywnie uczestniczy w zażartych dyskusjach i głosowaniach. Doceniamy Twoje nieustające wsparcie, dzięki któremu możemy razem rozwijać Polkadot i DeFi 🚀

# **Aktualizacja wydarzeń**

- **Unitize SF Blockchain Week**: Współzałożyciel Acala Bette Chen mówiła o tym jak działa między-sieciowe DeFi. Obejrzyj [powtórkę](https://next.brella.io/events/unitize2020/schedule/156155).
- **Defiant**: Ruitao Su i Bette Chen rozmawiali z Camila Russo o warstwie 0 na Polkadot, w jaki sposób ekosystem ewoluuje, tak aby mieć dużo i możliwie jak najwięcej łańcuchów pionowych specyficznych dla danej domeny. Podcast [tutaj](https://anchor.fm/camila-russo/episodes/Developers-Will-Wake-Up-to-the-Fact-That-Theres-a-Toolkit-to-Build-Full-Fledged-Customized-Chains-Acalas-Bette-Chen-eh7sp0/a-a2pmg6h) & czytaj [więcej](https://twitter.com/DefiantNews/status/1287758518913765377?s=20).
- Bette Chen jest wyjątkowa w **panelu Outlier Venture — „Prophesing the Future of Oracles”** obok MakerDAO, DIA, Set Protocol i Aave. Zobacz czat Bette na temat yield farming`u [tutaj](https://twitter.com/OVioHQ/status/1290644606892343297?s=20) & obejrzyj cały panel [powtórki](https://www.crowdcast.io/e/prophesying-oracles).

# O Acala

[ Acala ](http://acala.network/) to pierwsze w swoim rodzaju zdecentralizowane konsorcjum finansowe z wizją wprowadzenia stabilności finansowej, płynności i dostępności do głównego nurtu. **The Acala Network is a cross-chain finance hub for the Polkadot ecosystem** and beyond. Oferuje zestaw prymitywów finansowych: stablecoin z wieloma zabezpieczeniami wspierany przez aktywa międzyłańcuchowe, takie jak Bitcoin, niezaufany instrument pochodny do obstawiania i zdecentralizowana giełda, aby uwolnić płynność i napędzać innowacje finansowe. Jest to otwarta platforma dla dApps zorientowanych na finanse, którą można wdrożyć przy użyciu inteligentnych kontraktów lub wbudowanych protokołów z gotowymi funkcjami cross-chain, bezpieczeństwem i optymalizacjami finansowymi.

# Dołącz do nas

\[witryna internetowa\] (https://acala.network/) | \[Medium\] (https://medium.com/acalanetwork) | \[Twitter\] (https://twitter.com/AcalaNetwork) | \[GitHub\] (https://github.com/AcalaNetwork/Acala) | \[Acala Wiki\] (https://github.com/AcalaNetwork/Acala/wiki) | \[Discord\] (https://discord.gg/vdbFVCH) | \[Telegram\] (https://t.me/acalaofficial) | \[Riot Chat\] (https://riot.im/app/#/room/#acala:matrix.org)

Aby być na bieżąco z postępami w uruchomieniu Acali, zasubskrybuj \[Acala Newsletter\] (https: // share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

![Image for post](https://miro.medium.com/max/1500/0*1KozUmtgLB7qV79q.jpeg)

Acala jest dumnym stypendystą Web3 Foundation
