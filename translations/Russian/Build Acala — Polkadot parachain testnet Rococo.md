# Build Acala: тестовая парачейн-сеть Polkadot Rococo, сотрудничество с Ren, тестнет Mandala-мания, на The Defiant | Август 2020

Июль стал месяцем совместной работы с такими коллегами по экосистеме, как [ Ren](https://renproject.io/) и [ Laminar](http://laminar.one/), стресс-тестирование сети с десятками тысяч новых учетных записей и транзакций на протяжении всего Mandala Festival Season #3 и подготовка к запуску в тестовой парачейн-сети Polkadot Rococo.

![Изображение для публикации](https://miro.medium.com/max/8000/1*6wJEyP0ojcA8zM3SZAPzqQ.jpeg)

# **Обновления в девелопмент-сфере**

- ** Тестовая парачейн-сеть Polkadot ** [ ** Rococo: ** была запущена ](https://polkadot.network/introducing-rococo-polkadots-parachain-testnet/) ранее на этой неделе, что стало значительным шагом на пути к межсетевой интеграции. Парачейны теперь могут подключаться к релейной цепи, чтобы использовать ее общую безопасность, также доступна долгожданная передача сообщений между цепями, хотя она ограничена горизонтальной передачей сообщений, где релейная цепь будет использоваться для маршрутизации сообщений между двумя парачейнами. Acala работает над регистрацией на Rococo, чтобы проверить функциональность.
- [** Модуль RenVM-bridge **](https://github.com/AcalaNetwork/Acala/tree/master/ecosystem-modules) **и Интеграция renBTC: ** была развернута в тестовой сети Acala Mandala TC4, что стало первым шагом по внедрению renBTC в Acala и экосистему Polkadot. renBTC сейчас является токеном для комиссий, может использоваться в качестве обеспечения залога для займа стейблкоина и котируется на Acala DEX.
- ** Substrate RC4**: Mandala TC4 теперь обновлена до [ Substrate RC4](https://github.com/paritytech/substrate/releases/tag/v2.0.0-rc4), который позволяет атомарные транзакции - на один шаг ближе к готовым к применению смарт-контрактам и по завершении тестовой кампании будет обновлен до последней версии TC5.
- ** Acala Pulse**: аналитическая панель для отслеживания статистики сети находится в стадии разработки и будет выпущена на следующей неделе. Пользователи могут отслеживать основные параметры системы - выпуск aUSD, объем DEX и количество DOT в ликвидном стекинге, а также системные риски, ликвидации, аукционы и т. д.
- ** Моделирование "Черного четверга" и Аварийное отключение**: на следующей неделе [ в рамках Mandala Festival ](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#week-3-black-thursday-simulation) мы смоделируем волатильность в «черный четверг», протестируем гибридный механизм ликвидации, включающий DEX и аукционы для эффективного возврата кредитов. Затем мы задействуем систему Emergency Shutdown, обработаем все непогашенные займы и попросим пользователей вернуть свои залоговые средства из корзины активов. _ Festival week 3: правила и награды _ [_ здесь_](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#week-3-black-thursday-simulation) _._

  ![Изображение для публикации](https://miro.medium.com/max/2880/1*XQbgIIFPlzwrK8L1eXdKew.jpeg)

# **Обновления Экосистемы**

- [** Ren x Acala/Polkadot **](https://medium.com/acalanetwork/bringing-btc-to-polkadot-acala-x-ren-e7959855d5aa?source=collection_home---4------2-----------------------) ** ** для переноса Bitcoin и в будущем других изолированных классов активов на Acala и в более широкую мультичейновую вселенную Polkadot.
- [** Mandala Festival Season #3**](https://medium.com/acalanetwork/acala-mandala-festival-season-3-d0a6f155c154?source=collection_home---4------1-----------------------): начался две недели назад, вызвал большой ажиотаж: **_более 100 тыс. транзакций, 13 тыс. новых учетных записей, 2,5 + млн aUSD, выпущенных в результате обеспечения renBTC, и 250+ (тестовых) renBTC выпущено_**. Проверьте [действия на Subscan](https://acala-testnet.subscan.io/).
- [** Hackusama с Acala**](https://medium.com/acalanetwork/hackusama-ea1ddf3e945a): Acala является партнером Hackusama по обучению, предоставляя все паллеты времени выполнения и [ общие библиотеки](https://github.com/open-web3-stack/open-runtime-module-library), такие как оракулы и паллеты с несколькими токенами, техническую поддержку и советы для команд, создающие проекты DeFi.
- ** Acala Foundation теперь является членом совета** на Polkadot, активно участвуя в Polkadot Direction riot discussion и голосовании. Мы ценим вашу постоянную поддержку, благодаря ей мы можем вместе развивать Polkadot и DeFi 🚀

# **Анонсы Мероприятий**

- ** Unitize SF Blockchain Week**: соучредитель Acala Бетт Чен рассказала о кросс-чейн DeFi в действии. Посмотреть запись можно [здесь](https://next.brella.io/events/unitize2020/schedule/156155).
- ** The Defiant**: Руитао Су и Бетт Чен побеседовали с Камилой Руссо о том, что Polkadot находится на уровне 0, как экосистема развивается, чтобы иметь множество доменных вертикалей цепей и многое другое. Подкаст [ здесь](https://anchor.fm/camila-russo/episodes/Developers-Will-Wake-Up-to-the-Fact-That-Theres-a-Toolkit-to-Build-Full-Fledged-Customized-Chains-Acalas-Bette-Chen-eh7sp0/a-a2pmg6h) и читать [ подробнее](https://twitter.com/DefiantNews/status/1287758518913765377?s=20).
- Бетт Чен выделяется на дискуссионной панели ** Outlier Venture - «Prophesying the Future of Oracles» ** вместе с MakerDAO, DIA, Set Protocol и Aave. Смотрите речь Бетт о доходном фарминге[ здесь](https://twitter.com/OVioHQ/status/1290644606892343297?s=20), а также ознакомьтесь с полной [ записью](https://www.crowdcast.io/e/prophesying-oracles).

# Об Acala

[ Acala](http://acala.network/) - это первый в своем роде консорциум децентрализованного финансирования, который стремится обеспечить финансовую стабильность, ликвидность и доступность для всех. **Acala Network - это межсетевой финансовый центр для экосистемы Polkadot** и не только. Он предлагает набор финансовых примитивов: стейблкоин с множественным обеспечением, поддерживаемый кросс-чейновыми активами, такими как Bitcoin, производный инструмент без доверия и децентрализованный обмен для раскрытия ликвидности и поддержки финансовых инноваций. Это открытая платформа для ориентированных на финансы dApps, для развертывания с использованием смарт-контрактов или встроенных протоколов с готовыми возможностями кросс-чейна, безопасностью и финансовой оптимизацией.

# Присоединяйтесь к нам

[Website](https://acala.network/) | [Medium](https://medium.com/acalanetwork) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

Чтобы быть в курсе процесса запуска Acala, подпишитесь на [новостную рассылку Acala](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

![Изображение для публикации](https://miro.medium.com/max/1500/0*1KozUmtgLB7qV79q.jpeg)

Acala гордится полученным грантом от Web3 Foundation
