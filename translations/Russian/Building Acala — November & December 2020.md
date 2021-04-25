# Building Acala — ноябрь и декабрь 2020

## Краткий обзор Краудлоан и Парачейн аукцион Karura, EVM, Ampleforth, Open Oracle Gateway для Polkadot и другие новости

![Изображение для публикации](https://miro.medium.com/max/1600/0*FFQACU02-W0imy_8)

Счастливых праздников! Это специальный выпуск Building Acala, в котором представлены обновления за ноябрь и декабрь 2020 года. Если вы новичок в Acala, добро пожаловать! [ Acala ](http://acala.network/) - это децентрализованный финансовый центр Polkadot, который позволяет быстро и легко использовать или создавать финансовые приложения, повышая эффективность торговли и экономя драгоценное время.

Последние пару месяцев были посвящены созданию и возвращению - мы совершили значительный прорыв в возможности компоновки и совместимости EVM и Substrate, развернули Open Oracle Gateway с Acala, Band и DIA в качестве первых поставщиков сети оракулов, приветствовали присоединение Ampleforth к экосистеме и AMPL в Acala / Polkadot и запустил краудлоан-кампанию Karura (DeFi-центр Kusama) в преддверии предстоящего аукциона парачейнов и запуска.

# Новости в сфере исследований и девелопмента

- ** Project Bodhi ** - это объединяемый и инновационный стек EVM на Substrate, обеспечивающий возможность компоновки полного стека между EVM и средами выполнения для разработчиков, а также возможность кросс-чейна с одним кошельком для пользователей. Подробнее [на Github](https://github.com/w3f/Open-Grants-Program/blob/master/applications/project_bodhi.md). Дальнейшие подробности будут раскрыты в следующей публикации и демо.
- ** Open Oracle Gateway ** - это наш подход к созданию более открытой, инклюзивной и децентрализованной среды оракулов для DeFi-центра Acala, экосистем Polkadot, Kusama и других. Шлюз позволяет нескольким сетям оракулов предоставлять услуги любым DApps, развернутым или подключенным к Acala, при этом обеспечивая качество обслуживания и бесплатные комиссии за транзакции. Шлюз запущен и работает в тестовой сети Acala. Acala, Band и DIA являются первыми поставщиками сети оракулов. Ниже вы найдете более подробную информацию:

  [Представляем Open Oracle Gateway для Polkadot](https://medium.com/acalanetwork/introducing-the-open-oracle-gateway-for-polkadot-3554f7a4254e)

  ![Изображение для публикации](https://miro.medium.com/max/3200/0*vgXF6h9S3o0-qMgL)

- ** Ampleforth на Acala / Polkadot **: AMPL - перебазированная валюта и строительный блок эластичного финансирования, будет доступен на Polkadot через сеть Acala. Ample станет токеном первого класса для комиссии на Acala, контракты Ampleforth будут развернуты на EVM Acala с минимальными изменениями, при этом благодаря Project Bodhi будет обеспечена беспрепятственная интеграция с примитивами DeFi и ликвидностью Acala. Ниже вы найдете более подробную информацию:

  [Ampleforth, строительный блок DeFi, перебазирует валютные и эластичные финансы в Acala и…](https://medium.com/acalanetwork/ampleforth-a-defi-building-block-brings-rebasing-currency-and-elastic-finance-to-acala-and-fd1388e8e8fc)

- ** Децентрализованный суверенный фонд благосостояния ** - это DAO следующего поколения и нефоркаемый AUM. Подробнее читайте ниже и на [блоге Parity](https://www.parity.io/defi-on-polkadot-an-ecosystem-overview/#:~:text=Polkadot%20%2D%20a%20network%20protocol%20that,to%20be%20transferred%20across%20blockchains.).

  [Децентрализованный фонд суверенного благосостояния Acala - новое поколение DAO и Unforkable AUM](https://medium.com/acalanetwork/acalas-decentralized-sovereign-wealth-fund-a-next-gen-dao-unforkable-aum-80f8c23d8f27)

- ** Аудит безопасности: ** SRLabs и Slow Mist завершили свои аудиты по Acala, включая все реализации среды выполнения, модуль экосистемы RenVM, поддерживаемые сообществом модули ORML, от которых зависит Acala, а также внешний интерфейс для DApp Acala. Аудит Trail of Bits планируется начать в январе 2021 года. Ниже вы найдете более подробную информацию:

  [Аудит безопасности Acala](https://medium.com/acalanetwork/acala-security-audit-edd1850e27aa)

# План запуска и Сообщество

- ** График запуска: ** Выпущена тестовая сеть Rococo parachain V1, которая будет принимать парачейны в начале января 2021 года. Это надежный технический индикатор готовности парачейнов. Если тестирование и аудит пойдут по плану, то Kusama включит аукционы парачейнов, а затем Polkadot. Acala будет одним из первых парачейнов и запустится в обеих сетях.

  ![Изображение для публикации](https://miro.medium.com/max/2376/1*a-5oImcqeMrXczG4RZK7-Q.png)

- ** Открыт список ожидания краудлоана для запуска парачейна от Karura: ** Karura (сестринская сеть Acala на Kusama) проведет первый запуск краудсорсингового парачейна. Модель ** Crowdloan ** является пионером нового способа справедливой начальной загрузки сети: держатели KSM лочат свои токены, чтобы помочь нам арендовать слот парачейна и получить доступ к общей безопасности Kusama, которые будут возвращены им в конце аренды, дополнительно будут получены токены KAR, в качестве вознаграждения за их поддержку. Цель состоит в том, чтобы раздать наши токены как можно большему количеству держателей KSM, и для достижения этой цели создана бонусная реферальная программа. Кампания началась несколько дней назад, и уже привлекла ** _ 3,3 тысячи человек, присоединившихся к списку ожидания Crowdloan! _ Присоединяйтесь к списку ожидания Crowdloan Karura ** [** здесь **](https://twitter.com/AcalaNetwork/status/1339431441139154945?s=20) и просмотрите Karura Crowdloan [ сайт ](https://acala.network/kar-crowdloan).

- ** Substrate Runtime Developer Academy **, созданная Acala, Industry Connect и Parity и поддерживаемая широким кругом партнеров по сообществу, представляет собой программу профессионального уровня, помогающую разработчикам создавать производственные приложения для Polkadot. В первый набор вошли 52 студента из 19 стран, включая Аргентину, Бразилию, Россию, США, Турцию и другие страны. Казначейство Polkadot недавно предоставило программе стипендиальный фонд в размере 643 DOT для поддержки нуждающихся студентов. ** Узнайте больше ** [** о предложении Казначейства **](https://polkadot.polkassembly.io/treasury/28) ** или ** [** регистрируйтесь в следующую группу участников (февраль 2021 г.) прямо сейчас **](https://www.industryconnect.org/substrate-runtime-developer-academy/) **! **

- ** Проголосуйте за Acala в качестве члена совета Polkadot и Kusama: ** для более просвещенного будущего DeFi. За время нашей работы мы приняли участие в 37 голосах совета Kusama и 37 голосах совета Polkadot.

- ** Распределение токенов: ** одна из наших целей - максимально широко и справедливо распределить наши токены. В прошлом 2020 году, мы раздали сообществу примерно 100 тысяч токенов ACA и 3,5 миллиона KAR через участие в тестовой сети Mandala, программах баунти и призы на хакатонах.

# Мероприятие и СМИ

- ** Polkadot Decoded: ** первая конференция Polkadot собрала более 6000 участников, посмотрите презентацию соучредителя Acala Руитао Су можно[ здесь ](https://twitter.com/AcalaNetwork/status/1334596628951355392?s=20).
- ** Хакатоны: ** мы поддержали следующие хакатоны:
- Polkadot’s Hello World [на Gitcoin](https://gitcoin.co/hackathon/polkadot/?)
- Polkadot Encode Hackathon [здесь](https://medium.com/encode-club/encode-hack-club-announcing-polkadot-c7cc6cc12920)
- Substrate Dorahacks в Ханчжоу [здесь](https://twitter.com/DoraHacks/status/1339926282797105152?s=20)
- Соучредитель Acala Руитао во время конференц-связи с Pantera «Deconstructing DeFi» с соучредителем Alchemy Джо Лау [ здесь ](https://twitter.com/PanteraCapital/status/1323258191841558531?s=20)
- [ Стартап DeFi Acala для создания новой сети оракулов для экосистемы Polkadot ](https://coinmarketcap.com/zh/headlines/news/defi-startup-acala-to-build-new-oracle-network-for-polkadot-ecosystem/) от CoinMarketCap
- [DeFi on Polkadot](https://cointelegraph.com/news/defi-on-polkadot-an-alt-chain-with-interoperability-on-the-horizon) от Cointelegraph

<img alt="Изображение для публикации" class="t u v hu aj" src="https://miro.medium.com/max/2136/0\*-urwFFbwsGGsBSk8" width="1068" height="1600" srcSet="https://miro.medium.com/max/552/0\*-urwFFbwsGGsBSk8 276w, https://miro.medium.com/max/1104/0\*-urwFFbwsGGsBSk8 552w, https://miro.medium.com/max/1280/0\*-urwFFbwsGGsBSk8 640w, https://miro.medium.com/max/1400/0\*-urwFFbwsGGsBSk8 700w" sizes="700px" />

# Присоединяйтесь к нам

[Discord](https://discord.gg/vdbFVCH) | [Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

Чтобы быть в курсе того, как запускаются парачейны Acala на Polkadot и Kusama, подпишитесь на [новостную расслыку от Acala ](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

[Работа с нами](https://jobs.lever.co/acala/) — У нас есть вакансии 😎

# Об Acala

[ Acala ](http://acala.network/) - это децентрализованный финансовый центр Polkadot, который позволяет быстро и легко использовать или создавать финансовые приложения, повышая эффективность торговли и экономя драгоценное время. Платформа предлагает набор финансовых примитивов: стейблкоин с множественным обеспечением, поддерживаемый кросс-чейновыми активами, такими как Bitcoin, децентрализованная биржа и финансовых инноваций. Acala - это, де-факто, открытая платформа для финансовых приложений, использующая смарт-контракты или встроенные протоколы с готовыми возможностями кросс-чейна, безопасностью и финансовой оптимизацией.

# О Karura

[ Karura ](http://acala.network/karura-crowdloan) - это универсальный DeFi-центр в Kusama. Karura является сестринской сетью Acala с практически тем же кодом - обе платформы обеспечивают масштабируемую, удобную и быструю кросс-чейн экосистему DeFi для Kusama и Polkadot. Парачейн Karura - это динамичная и мощная платформа, которая позволяет создавать эффективные и недорогие финансовые приложения, повышая эффективность торговли и экономя время. Платформа предлагает набор финансовых примитивов: стейблкоин с множественным обеспечением, поддерживаемый кросс-чейновыми активами, такими как Kusama и Bitcoin, стейкинг и децентрализованная биржа для поддержки финансовых инноваций.
