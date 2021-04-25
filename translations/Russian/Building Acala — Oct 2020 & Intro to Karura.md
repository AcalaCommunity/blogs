# Building Acala - октябрь 2020 г. | Знакомство с Karura —  центром DeFi Kusama, Аренда Парачейнов (PLO) и Интеграция с EVM

![Изображение для публикации](https://miro.medium.com/max/1600/0*hmK9ex3hJqibgvrl)

Пришло время для редакции ** Building Acala ** за октябрь 2020 г., и если вы новичок в Acala, добро пожаловать! [ Acala ](http://acala.network/) - это децентрализованный финансовый центр Polkadot, который позволяет быстро и легко использовать или создавать финансовые приложения, повышая эффективность торговли и экономя драгоценное время.

В прошлом месяце команда работала над интеграцией EVM, поддерживала команды, развертывающие на Acala и запускала Karura - DeFi Hub Kusama через Parachain Lease Offering (PLO) и Paradrop.

# **Обновления в девелопмент-сфере**

- ** Совместимость с Ethereum и смарт-контракты **: мы разработали дальнейшую интеграцию EVM и смарт-контрактов с Acala. Отличие заключается в том, что контракты _ больше не находятся в изолированной программной среде (песочнице), но могут составляться с примитивами Acala DeFi _ (стейблкоин, DEX, стейкинг и другие), _ подключаться к базе пользователей Acala, ликвидность и возможности кросс-чейн, _ и открывает двери на гораздо более крупный рынок в экосистеме парачейнов Polkadot. Более подробная информация будет опубликована в ближайшее время.

- ** Аудит безопасности: ** мы завершили 2/3 запланированных аудитов безопасности, включая один аудит от SRLabs и предстоящий аудит от Trail of Bits. Более подробная информация об этом будет опубликована в ближайшие недели.

- ** Поддержка NFT: ** Acala построила общую [ NFT-паллету ](https://github.com/open-web3-stack/open-runtime-module-library/tree/master/nft) (также известную как модуль) для поддержки инноваций NFT в Acala, например, Rarible или другие поставщики NFT могут легко развернуть смарт-контракты, чтобы использовать строительные блоки DeFi Acala. Kusama приняла тот же модуль, чтобы включить встроенную поддержку NFT в цепи Kusama Relay. Подробнее [здесь](https://kusama.polkassembly.io/post/303#86924943-429c-4c05-a2fe-e7bef735b2a4).

# **Обновления о запуске**

- ** Acala запустит сеть Karura на Kusama (** [** Medium **](https://medium.com/acalanetwork/introducing-karura-acalas-defi-parachain-on-kusama-af2f2695b07a) **) ** - Karura является сестринской сетью Acala и центром DeFi для Kusama. Процесс запуска на Kusama может занять месяц или около того, хорошим сигналом будет готовность функциональности парачейна к тестовой сети Rococo.

- Karura проведет первое ** предложение аренды слота парачейна (PLO) ** и ** парадроп (** [** Medium **](https://medium.com/acalanetwork/karuras-approach-to-the-upcoming-parachain-lease-offering-plo-on-kusama-12fbf09ee463) **, ** [** Tweet **](https://twitter.com/KaruraNetwork/status/1319692583149457409?s=20) **) ** - Мы используем термин PLO, чтобы избежать путаницы, связанной с традиционным термином фондовой биржи «IPO». Karura будет использовать поддержку токенами KSM со стороны сообщества для участия в аукционе парачейнов. Затем эти KSM будут заблокированы на Kusama и возвращены участникам по окончании аренды слота парачейна. Karura предоставит участникам свой собственный токен KAR в качестве средства распределения токенов между сторонниками Kusama и Karura.

  ![Изображение для публикации](https://miro.medium.com/max/1600/1*EtNqbSOXqs4ZkljaR0Db7Q.jpeg)

# **Обновления Экосистемы**

- Acala была выбрана для участия в DeFi Alliance, чтобы помочь повысить ликвидность сети для DeFi Hub Polkadot ([** Medium **](https://medium.com/acalanetwork/acala-selected-for-the-defi-alliance-accelerator-to-help-build-deploy-and-grow-the-defi-hub-of-c1526008963e)). В предыдущем контингенте работают одни из лучших команд DeFi, такие как: 0x, dYdX, Kyber Network, IDEX, Opyn, Set Protocol и Synthetix.

- Мы приветствуем участников программы Acala Ecosystem Program: [ Bifrost ](http://bifrost.finance/) - протокол распределения ликвидности между цепями, который интегрирует доллар Acala (aUSD) в качестве токена базовой валюты; [ Interlay ](https://polkadot.network/bitcoin-is-coming-to-polkadot/?utm_content=142539261&utm_medium=social&utm_source=twitter&hss_channel=tw-1595615893) - мост Bitcoin-Polkadot без доверия, который будет иметь дополнительные варианты использования PolkaBTC, aUSD и LDOT; [ Zenlink ](https://www.zenlink.pro/) - межсетевой протокол DEX, который будет сотрудничать и интегрироваться с Acala.

- Acala помогла запустить [ Substrate / Polkadot Developer Academy ](http://.guru/polkadot-substrate) ([** Tweet **](https://twitter.com/AcalaNetwork/status/1320921071835435008?s=20) **, ** [** Website **](http://ic.guru/polkadot-substrate)) - 6-недельный курс + практический проект для подготовки опытных разработчиков к профессиональной карьере в Substrate / Polkadot или стартапам. Программа разработана обучающей организацией MVP Studio, запущена с Parity и Polkadot, преподается соучредителем Acala / Laminar Брайаном Ченом и одобрена доктором Гэвином Вудом. Каждый, кто серьезно относится к строительству в пространстве Polkadot / Kusama / Substrate, должен посмотреть [ этот](http://ic.guru/polkadot-substrate) и этот [ твит ](https://twitter.com/AcalaNetwork/status/1320921071835435008?s=20).

  ![Изображение для публикации](https://miro.medium.com/max/5760/1*FajicLqehWMEzaUPx7ujjw.png)

# **Мероприятия**

- На ** Sub0 - Substrate Developer Conference **: Брайан Чен, соучредитель Acala, и Дэн Форбс, адвокат разработчиков из Parity, продемонстрировали создание собственного блокчейна менее чем за час. Посмотреть запись можно [здесь](https://t.co/XTLRKg8nZM?amp=1).

- **Polkadot’ Hello World! Gitcoin Challenge ** уже идёт, ознакомьтесь с Acala Challenge [ здесь ](https://t.co/tzL4gpN5FJ?amp=1).

- Бетт Чен, соучредитель Acala, была участницей подкаста Web3 Founders Venture - ** Создание субстрата DeFi для Polkadot **. Посмотреть запись можно [здесь](https://www.youtube.com/watch?v=aueB19YH19g&list=UUd_K-AgiS2XV8_iuRQ7JyNQ).

- Руитао Су, соучредитель Acala, был на дискуссии ** Crypto Tonight «Yes, Polkadot!» ** вместе с Фабианом Гомпфом из Parity, Джеком Платтсом из Hypersphere, Шилянг Тан из Ledger Prime. Посмотреть запись можно [здесь](https://www.youtube.com/watch?v=xXgtpcf9NVE&feature=youtu.be).

- Acala примет участие в Shanghai Blockchain Week 2020 в качестве спонсора хакатона и приглашенного докладчика. Зарегистрироваться можно [здесь](https://www.eventbrite.com/e/the-6th-global-blockchain-summit-tickets-115473469255).
- Руитао Су будет выступать на ** Polkadot Decoded - the Polkadot Community Conference ** ** 3 декабря ** вместе с доктором Гэвином Вудом, Юттой Штайнер, Камилой Руссо, Лаурой Шин и другими участниками, которые будут оглашены позже. Зарегистрироваться можно [здесь](https://t.co/BWUXh8dwf2?amp=1)

  ![Изображение для публикации](https://miro.medium.com/max/1360/0*bb5Vh6rDQWQihkX0)

# Присоединяйтесь к нам

[Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Discord](https://discord.gg/vdbFVCH) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

Чтобы быть в курсе того, как запускаются парачейны Acala на Polkadot и Kusama, подпишитесь на [новостную расслыку от Acala ](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

[**Работайте с нами.**](https://jobs.lever.co/acala/)

# Об Acala

[ Acala ](http://acala.network/) - это децентрализованный финансовый центр Polkadot, который позволяет быстро и легко использовать или создавать финансовые приложения, повышая эффективность торговли и экономя драгоценное время. Платформа предлагает набор финансовых примитивов: стейблкоин с множественным обеспечением, поддерживаемый кросс-чейновыми активами, такими как Bitcoin, децентрализованная биржа и финансовых инноваций. Acala - это, де-факто, открытая платформа для финансовых приложений, использующая смарт-контракты или встроенные протоколы с готовыми возможностями кросс-чейна, безопасностью и финансовой оптимизацией.
