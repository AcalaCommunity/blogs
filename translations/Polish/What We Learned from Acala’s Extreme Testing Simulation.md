# Czego nauczyliśmy się z symulacji ekstremalnych testów Acala

## Trzytygodniowa kampania sieci testowej Acala dobiegła końca, podkreślając znaczenie sieci ostrzegawczej i prowadząc do kilku technicznych ulepszeń sieci

![Obraz do wpisu](https://miro.medium.com/max/1600/1*lGVbzGOgp5M3DqCPtAds8A.jpeg)

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
- **Wysoka przepustowość i specjalizacja:** Acala posiada niezoptymalizowaną przepustowości 1000 tps; w wielołańcuchowym świecie Polkadot, każda część/parachain zostanie prawdopodobnie zoptymalizowany pod kątem jego zastosowań. Na przykład Acala będzie częścią finansową zoptymalizowaną pod kątem operacji DeFi, podczas gdy inna sieć może się specjalizować w grach lub hodowli kotów. Rzeczywista przepustowość Polkadot mogłaby wynosić 1000 tps pomnożonych przez całkowitą liczbę połączonych części/parachain`ów.

Podczas kampanii, Acala prowadziła ćwiczenia Czarnego Czwartku w celu symulacji silnej zmienności cen skutkującej likwidacją ryzykownych pozycji kredytowych, po której następuje awaryjne wyłączenie systemu. Pod dużym obciążeniem system działał zgodnie z oczekiwaniami i ostatecznie wszystkie pożyczki zostały przetworzone, a zabezpieczenia zwrócono użytkownikom.

📉 ponad 14400 pożyczek zostało zlikwidowanych

⚡ zlikwidowano środki o wartości 1,37 miliona dolarów

# Siła płynności międzysieciowej

Acala jest to centrum finansowe wielo-sieciowego świata Polkadot. Dostarcza zestawu narzędzi finansowych, w tym wielozabezpieczony stablecoin, instrument pochodny staking`u bez powiernictwa oraz zdecentralizowaną wymianę. Narzędzia te są oferowane za pośrednictwem DApp Acali bezpośrednio użytkownikom końcowym, a także jako zestawy SDK do tworzenia większej liczby DApps. Widzimy bardziej połączony, autonomiczny, wyrafinowany, międzyblokowy ekosystem finansowy, który jest bardziej zintegrowany w sytuacjach kryzysowych.

Zintegrowaliśmy się z Ren i Laminar i pokazaliśmy moc między-sieciowej płynności:

₿ 1,403 renBTC zostało wybite

👨‍🌾 sprzedano renBTC o wartość 1,4 miliona USD na DeX`ie, a 5,5 miliona Usd zostało wykorzystanych do zawarcia pożyczek

🌈 4,3 mln aUSD przesłano do Laminar jako depozyt zabezpieczający (forex, złoto, syntetyczny BTC & ETH) handel z dźwignią

Dowiedz się więcej o zastosowaniach Acala między-sieciowego DeFi [tutaj](https://github.com/AcalaNetwork/Acala/wiki/T.-Cross-chain-DeFi); przyjdź i utwórz następny projekt DeFi za pomocą naszych frameworków, narzędzi DeFi oraz SDK. Nasze propozycje są jakości produkcyjnej i są gotowe do produkcji. Byliśmy również partnerem edukacyjnym w niedawnym wydarzeniu Hackusama w Kusamie i możesz dowiedzieć się więcej o budowaniu z Acalą [tutaj](https://medium.com/acalanetwork/hackusama-ea1ddf3e945a).

# Dołącz do nas

[Strona internetowa](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

Aby być na bieżąco z postępami w uruchamianiu Acali, zasubskrybuj [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).
