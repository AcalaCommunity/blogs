# Building Acala - сентябрь 2020 г. | Парачейн тестовой сети Acala, новый раунд финансирования, смарт-контракты и совместимость с Ethereum

![Изображение для публикации](https://miro.medium.com/max/1600/0*rPcIWxu2NiMMUEpU)

Пришло время для сентябрьской версии 2020 года ** Building Acala ** и, если вы новичок в Acala, добро пожаловать! [ Acala ](http://acala.network) - это децентрализованный финансовый центр Polkadot, который позволяет быстро и легко использовать или создавать финансовые приложения, повышая эффективность торговли и экономя драгоценное время. Оглядываясь назад на август, это был месяц, отмеченный важными результатами: парачейн Acala начал функционировать и успешно завершил передачу токенов в тестовой сети Polkadot, новый раунд инвесторов и стратегических партнеров, а также открытие смарт-контрактов и совместимости с Ethereum на Acala. Продолжайте следить за всеми событиями вокруг экосистемы Acala, а также мы приглашаем вас присоединиться к нам в [Twitter](https://twitter.com/acalanetwork) и [Telegram](https://t.me/AcalaOfficial).

# **Обновления в девелопмент-сфере**

- ** Acala представляет смарт-контракты и совместимость с Ethereum для Polkadot DeFi ** [**(Medium)**](https://medium.com/acalanetwork/acala-unveils-smart-contracts-and-ethereum-compatibility-for-polkadot-defi-588b3891e53d)**:** Acala теперь поддерживает EVM и подписи! паллеты на Substrate, что позволяет разработчикам использовать смарт-контракты на основе Solidity и Wasm.

- ** Acala запустила первый парачейн в тестовой сети Polkadot ** [ (**Medium**)](https://medium.com/acalanetwork/acala-launches-the-1st-parachain-on-polkadot-testnet-682c02bad08b): Acala запустила свой парачейн в тестовой сети Polkadot в рамках подготовки к развертыванию основной сети на Kusama и Polkadot.

- ** Первая успешная кросс-чейн передача токенов и торговля ими в Acala DEX ** [(**Twitter**)](https://twitter.com/AcalaNetwork/status/1297851737525481473?s=20): Acala включила полный пакет DeFi в парачейне тестовой сети: тестовые токены DOT можно без доверия передать в парачейн Acala, использовать в качестве базового токена комиссии и использовать для участия в DeFi, например: используйте для торговли на DEX или обеспечения кредитов в долларах США.

- ** Первый успешный кросс-чейн перенос стейблкоинов из Acala в Laminar в тестовой сети ** [(**Twitter**)](https://twitter.com/bettechentt/status/1298768242333237248?s=20): Acala интегрирована с [ Laminar](https://www.laminar.one/) в тестовой сети парачейна для надежной кросс-чейн передачи токенов и функциональности DeFi. Демо-видео:

- ** Acala построила и выпустила паллету _xtoken_ для передачи токенов в экосистеме Polkadot ** [(**Github**)](https://github.com/open-web3-stack/open-runtime-module-library/tree/rococo/xtokens): любой парачейн, использующий паллету xtoken, созданный Acala, теперь может интегрироваться с Acala для передачи токенов. Xtoken был выпущен как обычная хорошая библиотека для использования любым парачейном.

- ** Acala создала и выпустила код, чтобы помочь любой цепи на основе Substrate стать парачейном на Polkadot или Kusama ** [(**Github**)](https://github.com/AcalaNetwork/Acala/pull/362): ознакомьтесь с этим PR выше вместе с продолжающейся деятельностью по рефакторингу ([**Github**](https://github.com/AcalaNetwork/Acala/compare/rococo-rc6)) для поддержки цепей, работающих как независимые Substrate чейны или парачейны.

**Остальные предстоящие девелопмент-обновления:**

- Следующая версия тестовой сети Acala обеспечит возможность использование смарт-контрактов в Acala с рекомендациями по процессу производственной готовности
- Следите за появлением в ближайшее время большей интеграции кросс-парачейнов и кросс-блокчейнов

# **Обновления Экосистемы**

- **Acala создает дополнительную Серию A для Polkadot DeFi Hub в преддверии предстоящего запуска Parachain (**[**Medium**](https://medium.com/acalanetwork/acala-raises-additional-series-a-for-polkadot-defi-hub-ahead-of-upcoming-parachain-launch-22fdee9c2be9)**)**: Acala собрала дополнительный раунд финансирования вместе с партнерскими отношениями для экспертной оценки DeFi, обеспечения ликвидности и управления рисками ([Twitter](https://twitter.com/bettechentt/status/1299497896207773696?s=20)).
- ** Что мы узнали из моделирования экстремального тестирования Acala **([Средний](https://medium.com/acalanetwork/what-we-learned-from-acalas-extreme-testing-simulation-5ef5769a0902)): трехнедельная кампания тестовой сети Acala завершилась, подчеркнув важность канареечной сети и приведя к нескольким техническим улучшениям в сеть.

Некоторые статистические данные, которые мы наблюдали во время этой кампании сообщества по тестированию:

✅ 14,500 + новых аккаунтов | ⛓️ 140,000 + значимых транзакций | 💰 $52 миллионов залочено всего | 💲 $25 миллионов aUSD сминтенно

Ниже приведены основные награды, а полные результаты опубликованы на [ Github ](https://github.com/AcalaNetwork/Acala/wiki/W.-Contribution-&-Rewards#season-3-prize-giving):

😎 Награды 1-ой недели получили 2105 пользователей из 10 525 прошедших квалификацию

⌛ Награды 2-ой недели получили 10 лучших трейдеров со средней доходностью в 24 200%

🌋 Награды 3-ей недели получили 200 пользователей

✍️ Награждены были 10 блогеров / влогеров

🐞 Награждено 45 баг-хантеров

🤖️ Присуждена 1 награда за кодировку

# **Acala в СМИ**

![Изображение для публикации](https://miro.medium.com/max/2576/1*v2Ndsw3UwNTj0EhQNbFykw.png)

[CoinDesk](https://www.coindesk.com/acala-polkadot-defi-7m-pantera-saft)

![Изображение для публикации](https://miro.medium.com/max/2562/1*z4iztwspAQT0KgfGt4jp_w.png)

[Yahoo Finance](https://finance.yahoo.com/news/polkadot-based-defi-project-acala-092543143.html)

![Изображение для публикации](https://miro.medium.com/max/2274/1*ZA2JHJmNc15TXwClrwE_GQ.png)

[CryptoBriefing](https://cryptobriefing.com/acala-network-polkadots-makerdao-comes-ethereum/)

# **Мероприятия**

- [Acala участвовала в кросс-чейн DeFi AMA с Acala, Laminar и Ren на 650+ человек](https://twitter.com/AcalaNetwork/status/1295477682214338560?s=20)
- 16–18 сентября: Acala выступила на 3-ем Китайском международном саммите по развитию будущего блокчейн-бизнеса, организованном Chain News и inkrpto
- Соучредитель Acala Ruitao оценил первый хакатон Kusama, а также поддержал Hackusama и Acala в качестве партнера по технологиям и обучению ([Hackusama with Acala](https://medium.com/acalanetwork/hackusama-ea1ddf3e945a)). Хоть этот хакатон и закончился, но строительство продолжается! Мы ищем отличные команды, создающие продукты, связанные с DeFi или финансами. Приходите строить с Acala ([Github - Build with Acala](https://github.com/AcalaNetwork/Acala/wiki/U.-Build-with-Acala)).

![Изображение для публикации](https://miro.medium.com/max/1358/0*qMAanMu2kGLUXByX)

# Присоединяйтесь к нам

[Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

Чтобы быть в курсе того, как запускаются парачейны Acala на Polkadot и Kusama, подпишитесь на новостную рассылку от

 Acala.</p> 



# **Об Acala**

[ Acala](http://acala.network/) - это децентрализованный финансовый центр Polkadot, который позволяет быстро и легко использовать или создавать финансовые приложения, повышая эффективность торговли и экономя драгоценное время. Платформа предлагает набор финансовых примитивов: стейблкоин с множественным обеспечением, поддерживаемый кросс-чейновыми активами, такими как Bitcoin, децентрализованная биржа и финансовых инноваций. Acala - это, де-факто, открытая платформа для финансовых приложений, использующая смарт-контракты или встроенные протоколы с готовыми возможностями кросс-чейна, безопасностью и финансовой оптимизацией.
