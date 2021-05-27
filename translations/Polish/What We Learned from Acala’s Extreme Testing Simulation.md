# Czego nauczyliśmy się z symulacji ekstremalnych testów Acala

## Trzytygodniowa kampania sieci testowej Acala dobiegła końca, podkreślając znaczenie sieci ostrzegawczej i prowadząc do kilku technicznych ulepszeń sieci

![Image for post](https://miro.medium.com/max/1600/1*lGVbzGOgp5M3DqCPtAds8A.jpeg)

Autor: [Bette Chen](https://medium.com/u/8d475d21e811?source=post_page-----5ef5769a0902--------------------------------)

Acala [Mandala Fest Season #3](https://medium.com/acalanetwork/acala-mandala-festival-season-3-d0a6f155c154), 3-tygodniowa kampania sieci testowej została pomyślnie zakończona 17 sierpnia. Był to dla nas świetny sposób na pokazanie wspólnocie postępów naszego rozwoju poprzez testowanie systemu i protokołów pod ciężkimi obciążeniami i ekstremalnymi sytuacjami, przy jednoczesnym zapewnieniu nagród uczestnikom.

Zostaliśmy przytłoczeni wsparciem, entuzjazmem i udziałem społeczności. Oto niektóre statystyki:

✅ 14,500 + nowych kont

⛓️ ponad 140 000 znaczących transakcji

💰 łączna wartość zablokowanych środków to 52 miliony dolarów

💲 wyemitowane 25 mln aUSD

**Najważniejsze nagrody są następujące, natomiast pełne wyniki zostały opublikowane** [**tutaj**](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#season-3-prize-giving)****

😎 Nagrody w Tygodniu 1 trafiły do 2 105 użytkowników spośród 10 525 zakwalifikowanych

[⌛](https://emojipedia.org/hourglass-done/) Nagrody w Tygodniu 2 trafiły do pierwszych 10 traderów, ze średnim zwrotem 24,200%

🌋 Nagrody w Tygodniu 3 trafiły do 200 użytkowników

✍️ 10 bloggerów/vloggerów nagrodzonych

🐞 nagrodzono 45 łowców błędów

🤖 przyznano 1 nagrodę za kod

Wyciągnęliśmy również pewne cenne lekcje, z których część potwierdziła nasze precepcje, podczas gdy inne doprowadziły do poprawy.

# Znaczenie sieci ostrzegawczej "Canary Network"

Tradycyjne tworzenie sieci blockchain składa się tylko z sieci testowych oraz środowisk gotowych do produkcji. Uważamy jednak, że sieć blockchain nie może zostać odpowiednio przetestowany bez prawdziwych warunków ekonomicznych. Z kampanii sieci testowej Mandala jasno widać, że wraz ze sporadycznymi nagrodami (głównie poprzez losowanie szczęśliwych uczestników), w dużym stopniu można przetestować funkcjonalność i użyteczność, to dynamika gospodarcza, wydajność płynności oraz tolerancja na ryzyko nie może być w pełni zbadana w niemającej wartości sieci testowej, takiej jak Mandala.

Podobnie jak w przypadku sieci [Kusama](http://kusama.network) będącą siecią ostrzegawczą dla Polkadot, Acala zaimplementowała sieć ostrzegawczą [Karura](https://github.com/AcalaNetwork/Acala/wiki/1.-Get-Started#acala-trilogy-networks). Obie sieci mają realną wartość ekonomiczną, ale mniejszą niż sieć podstawowa (w naszym przypadku Acala). Sieć Karura ma wartość ekonomiczną reprezentowaną przez jej natywny token sieciowy [KAR](https://github.com/AcalaNetwork/Acala/wiki/V.-ACA-&-KAR); zostanie ona uruchomiona jako parachain w sieci Kusuma i zapewni prymitywy finansowe ekosystemowi Kusama, takie jak akceptacja KSM jako zabezpieczenia linii kredytowych dla stablecoin`ów.

# Wnioski z Symulacji Czarnego Czwartku - Płynność to Król

Być może doszliśmy do wniosku, że tolerancja na ryzyko finansowe zdecentralizowanego (opartego na blockchain) systemu finansowego jest w dużej mierze zdeterminowana przez możliwości i ograniczenia techniczne leżące u podstaw rejestru. Przedstawiliśmy podstawowe kwestie, które doprowadziły do incydentu MakerDAO, 12 marca Czarny Czwartek [tutaj](https://medium.com/acalanetwork/regaining-confidence-in-decentralized-stablecoins-bd98ba8e3c83):

- Przepustowości to wąskie gardło wydajności sieci
- Nieefektywność w likwidacji ryzykownych pożyczek zabezpieczonych lub kredytów CDP
- Niesprawność posiadaczy & kryzys płynności

## Wprowadziliśmy następujące ulepszenia:

- **Jakość usług dla operacji na wyroczniach:** transakcje na wyroczniach są traktowane priorytetowo i zawsze są zawarte w bloku, więc kanały cen są aktualne i nie wpływają na ruch sieciowy
- **Automatyczny likwidator** przy użyciu [Off-chain Workers](https://www.parity.io/substrate-off-chain-workers-secure-and-efficient-computing-intensive-tasks/): zewnętrzni gracze, tacy jak Keeperzy, są wymagani w protokołach takich jak Maker tylko dlatego, że Ethereum lub podobna technologia nie może zapewnić bezpiecznego automatycznego harmonogramu w węźle blockchain. Acala wdrożyła auto-likwidator, który może skutecznie oceniać pozycje kredytów w każdym bloku.
- **Hybrydowy mechanizm likwidacji z DEX`em i aukcją:** system automatycznie zlikwiduje zabezpieczenia na DEX`ie, jeżeli cena i jej "slippage" są korzystne, aby unikanąć nieefektywności cenowej aukcji.
- **Wysoka przepustowość i specjalizacja:** Acala posiada niezoptymalizowaną przepustowości 1000 tps; w wielołańcuchowym świecie Polkadot, każdy odłamek/parachain zostanie prawdopodobnie zoptymalizowany pod kątem jego zastosowań. Na przykład Acala będzie odłamkiem finansowym zoptymalizowanym pod kątem operacji DeFi, podczas gdy inna sieć może specjalizować się w grach lub hodowli kotów. Rzeczywista przepustowość Polkadot wyniosłaby 1000 tps pomnożone przez całkowitą liczbę połączonych odłamków / spadochronów.

Podczas kampanii Acala przeprowadziła wiertło Czarny Czwartek, aby zasymulować silną zmienność cen skutkującą likwidacją ryzykownych pozycji kredytowych, a następnie awaryjnym wyłączeniem systemu. Pod dużym obciążeniem system działał zgodnie z oczekiwaniami i ostatecznie wszystkie pożyczki zostały przetworzone, a zabezpieczenia zwrócono użytkownikom.

📉 14,400+ loans were liquidated

📉 Ponad 14 400 pożyczek zostało zlikwidowanych

# Siła płynności

międzyłańcuchowej Acala jest centrum finansowym wielobranżowego świata Polkadot. Zapewnia zestaw prymitywów finansowych, w tym multi-zabezpieczony stablecoin, bezzałogową pochodną do obstawiania i zdecentralizowaną giełdę. Te prymitywy są oferowane za pośrednictwem DApp firmy Acala bezpośrednio użytkownikom końcowym, a także jako zestawy SDK do tworzenia większej liczby DApps. Widzimy bardziej wzajemnie powiązany, autonomiczny, wyrafinowany ekosystem finansowy obejmujący wiele bloków blokowych na progu pojawienia się.

We have integrated with Ren and Laminar and showcased the power of cross-chain liquidity:

Zintegrowaliśmy się z Renem i Laminarem i zaprezentowaliśmy potęgę płynności:

międzyłańcuchowej₿ 1403 renBTC zostało wybite

👨‍🌾 1,4 miliona dolarów renBTC w obrocie na DeX, 5,5 miliona dolarów wykorzystane w pożyczkach

depozytemDowiedz się więcej na temat przypadków użycia cross-chain DeFi firmy Acala \[tutaj\] (https://github.com/AcalaNetwork/Acala/wiki/T.-Cross-chain-DeFi); przyjdź i stwórz kolejny zabójczy projekt DeFi, korzystając z naszego frameworka, prymitywów DeFi i SDK. Nasze oferty są przeznaczone do produkcji i gotowe do produkcji. Byliśmy również partnerem edukacyjnym podczas niedawnego wydarzenia Hackusama w Kusamie, a więcej o budowaniu z Acala możesz dowiedzieć się \[tutaj\] (https://medium.com/acalanetwork/hackusama-ea1ddf3e945a).

# Dołącz do nas

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

\[witryna internetowa\] (https://acala.network/) | \[Medium\] (https://medium.com/acalanetwork) | \[Twitter\] (https://twitter.com/AcalaNetwork) | \[GitHub\] (https://github.com/AcalaNetwork/Acala) | \[Acala Wiki\] (https://github.com/AcalaNetwork/Acala/wiki) | \[Discord\] (https://discord.gg/vdbFVCH) | \[Telegram\] (https://t.me/acalaofficial) | \[Riot Chat\] (https://riot.im/app/#/room/#acala:matrix.org)
