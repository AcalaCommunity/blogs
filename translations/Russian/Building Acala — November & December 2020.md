# Building Acala — ноябрь и декабрь 2020

## Краткий обзор Краудлоан и Парачейн аукцион Karura, EVM, Ampleforth, Open Oracle Gateway для Polkadot и другие новости

![Image for post](https://miro.medium.com/max/1600/0*FFQACU02-W0imy_8)

Счастливых праздников! Это специальный выпуск Building Acala, в котором представлены обновления за ноябрь и декабрь 2020 года. Если вы новичок в Acala, добро пожаловать! [ Acala ](http://acala.network/) - это децентрализованный финансовый центр Polkadot, который позволяет быстро и легко использовать или создавать финансовые приложения, повышая эффективность торговли и экономя драгоценное время.

Последние пару месяцев были посвящены созданию и возвращению - мы совершили значительный прорыв в возможности компоновки и совместимости EVM и Substrate, развернули Open Oracle Gateway с Acala, Band и DIA в качестве первых поставщиков сети оракулов, приветствовали присоединение Ampleforth к экосистеме и AMPL в Acala / Polkadot и запустил краудлоан-кампанию Karura (DeFi-центр Kusama) в преддверии предстоящего аукциона парачейнов и запуска.

# Новости в сфере исследований и девелопмента

- ** Project Bodhi ** - это объединяемый и инновационный стек EVM на Substrate, обеспечивающий возможность компоновки полного стека между EVM и средами выполнения для разработчиков, а также возможность кросс-чейна с одним кошельком для пользователей. Подробнее [на Github](https://github.com/w3f/Open-Grants-Program/blob/master/applications/project_bodhi.md). Дальнейшие подробности будут раскрыты в следующей публикации и демо.
- ** Open Oracle Gateway ** - это наш подход к созданию более открытой, инклюзивной и децентрализованной среды оракулов для DeFi-центра Acala, экосистем Polkadot, Kusama и других. Шлюз позволяет нескольким сетям оракулов предоставлять услуги любым DApps, развернутым или подключенным к Acala, при этом обеспечивая качество обслуживания и бесплатные комиссии за транзакции. Шлюз запущен и работает в тестовой сети Acala. Acala, Band и DIA являются первыми поставщиками сети оракулов. Ниже вы найдете более подробную информацию:

  [Представляем Open Oracle Gateway для Polkadot](https://medium.com/acalanetwork/introducing-the-open-oracle-gateway-for-polkadot-3554f7a4254e)

  ![Image for post](https://miro.medium.com/max/3200/0*vgXF6h9S3o0-qMgL)

- ** Ampleforth на Acala / Polkadot **: AMPL - перебазированная валюта и строительный блок эластичного финансирования, будет доступен на Polkadot через сеть Acala. Ample станет токеном первого класса для комиссии на Acala, контракты Ampleforth будут развернуты на EVM Acala с минимальными изменениями, при этом благодаря Project Bodhi будет обеспечена беспрепятственная интеграция с примитивами DeFi и ликвидностью Acala. Ниже вы найдете более подробную информацию:

  [Ampleforth, строительный блок DeFi, перебазирует валютные и эластичные финансы в Acala и…](https://medium.com/acalanetwork/ampleforth-a-defi-building-block-brings-rebasing-currency-and-elastic-finance-to-acala-and-fd1388e8e8fc)

- ** Децентрализованный суверенный фонд благосостояния ** - это DAO следующего поколения и нефоркаемый AUM. Подробнее читайте ниже и на [блоге Parity](https://www.parity.io/defi-on-polkadot-an-ecosystem-overview/#:~:text=Polkadot%20%2D%20a%20network%20protocol%20that,to%20be%20transferred%20across%20blockchains.).

  [Децентрализованный фонд суверенного благосостояния Acala - новое поколение DAO и Unforkable AUM](https://medium.com/acalanetwork/acalas-decentralized-sovereign-wealth-fund-a-next-gen-dao-unforkable-aum-80f8c23d8f27)

- ** Аудит безопасности: ** SRLabs и Slow Mist завершили свои аудиты по Acala, включая все реализации среды выполнения, модуль экосистемы RenVM, поддерживаемые сообществом модули ORML, от которых зависит Acala, а также внешний интерфейс для DApp Acala. Аудит Trail of Bits планируется начать в январе 2021 года. Ниже вы найдете более подробную информацию:

  [Аудит безопасности Acala](https://medium.com/acalanetwork/acala-security-audit-edd1850e27aa)

# План запуска и Сообщество

- ** График запуска: ** Выпущена тестовая сеть Rococo parachain V1, которая будет принимать парачейны в начале января 2021 года. Это надежный технический индикатор готовности парачейнов. Если тестирование и аудит пойдут по плану, то Kusama включит аукционы парачейнов, а затем Polkadot. Acala будет одним из первых парачейнов и запустится в обеих сетях.

  ![Image for post](https://miro.medium.com/max/2376/1*a-5oImcqeMrXczG4RZK7-Q.png)

- ** Открыт список ожидания краудлоана для запуска парачейна от Karura: ** Karura (сестринская сеть Acala на Kusama) проведет первый запуск краудсорсингового парачейна. Модель ** Crowdloan ** является пионером нового способа справедливой начальной загрузки сети: держатели KSM лочат свои токены, чтобы помочь нам арендовать слот парачейна и получить доступ к общей безопасности Kusama, которые будут возвращены им в конце аренды, дополнительно будут получены токены KAR, в качестве вознаграждения за их поддержку. Цель состоит в том, чтобы раздать наши токены как можно большему количеству держателей KSM, и для достижения этой цели создана бонусная реферальная программа. Кампания началась несколько дней назад, и уже привлекла ** _ 3,3 тысячи человек, присоединившихся к списку ожидания Crowdloan! _ Присоединяйтесь к списку ожидания Crowdloan Karura ** [** здесь **](https://twitter.com/AcalaNetwork/status/1339431441139154945?s=20) и просмотрите Karura Crowdloan [ сайт ](https://acala.network/kar-crowdloan).

- ** Substrate Runtime Developer Academy **, созданная Acala, Industry Connect и Parity и поддерживаемая широким кругом партнеров по сообществу, представляет собой программу профессионального уровня, помогающую разработчикам создавать производственные приложения для Polkadot. В первый набор вошли 52 студента из 19 стран, включая Аргентину, Бразилию, Россию, США, Турцию и другие страны. Казначейство Polkadot недавно предоставило программе стипендиальный фонд в размере 643 DOT для поддержки нуждающихся студентов. **Read more** [**on the Treasury proposal**](https://polkadot.polkassembly.io/treasury/28) **or** [**sign up for the next cohort (Feb 2021) now**](https://www.industryconnect.org/substrate-runtime-developer-academy/)**!**

- **Vote Acala for Polkadot & Kusama Council Member:** for a more enlightened DeFi future. During our tenure, we have participated in 37 Kusama council votes and 37 Polkadot council votes.

- **Token Distribution:** one of our goals is to distribute our tokens as widely and fairly as possible. Looking back 2020, we have distributed roughly 1 hundred thousand ACA and 3.5 million KAR tokens to the community through testnet participation — the Mandala Festivals, bounty programs and hackathon prizes.

# Events & Media

- **Polkadot Decoded:** the first Polkadot conference has attracted over 6,000 attendants, watch Acala’s co-founder Ruitao Su’s presentation [here](https://twitter.com/AcalaNetwork/status/1334596628951355392?s=20).
- **Hackathons:** we have supported the following hackathons:
- Polkadot’s Hello World [on Gitcoin](https://gitcoin.co/hackathon/polkadot/?)
- Polkadot Encode Hackathon [here](https://medium.com/encode-club/encode-hack-club-announcing-polkadot-c7cc6cc12920)
- Substrate Dorahacks in Hangzhou [here](https://twitter.com/DoraHacks/status/1339926282797105152?s=20)
- Acala’s co-founder Ruitao on Pantera’s Conference Calls “Deconstructing DeFi” with Alchemy’s co-founder Joe Lau [here](https://twitter.com/PanteraCapital/status/1323258191841558531?s=20)
- [DeFi Startup Acala to Build New Oracle Network For Polkadot Ecosystem](https://coinmarketcap.com/zh/headlines/news/defi-startup-acala-to-build-new-oracle-network-for-polkadot-ecosystem/) by CoinMarketCap
- [DeFi on Polkadot](https://cointelegraph.com/news/defi-on-polkadot-an-alt-chain-with-interoperability-on-the-horizon) by Cointelegraph

<img alt="Image for post" class="t u v hu aj" src="https://miro.medium.com/max/2136/0\*-urwFFbwsGGsBSk8" width="1068" height="1600" srcSet="https://miro.medium.com/max/552/0\*-urwFFbwsGGsBSk8 276w, https://miro.medium.com/max/1104/0\*-urwFFbwsGGsBSk8 552w, https://miro.medium.com/max/1280/0\*-urwFFbwsGGsBSk8 640w, https://miro.medium.com/max/1400/0\*-urwFFbwsGGsBSk8 700w" sizes="700px" />

# Join Us

[Discord](https://discord.gg/vdbFVCH) | [Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Telegram](https://t.me/acalaofficial) | [Riot Chat](https://riot.im/app/#/room/#acala:matrix.org)

To keep up to date with progress on the Acala parachain launches on Polkadot and Kusama, subscribe to the [Acala Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc).

[Work with us](https://jobs.lever.co/acala/) — we’re hiring 😎

# About Acala

[Acala](http://acala.network/) is the decentralized financial hub of Polkadot that makes it fast and easy to use or build financial applications, improving trading efficiency and saving valuable time. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de-facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities, security and financial optimizations.

# About Karura

[Karura](http://acala.network/karura-crowdloan) is the decentralized financial hub of Kusama. The network is built as Acala’s sister network with nearly the same codebase — the two platforms enable a scalable, user-friendly, and fast cross-chain DeFi ecosystem for Kusama and Polkadot. Karura’s parachain is a fast-moving and powerful platform that enables efficient, inexpensive, and sophisticated financial applications, improving trading effectiveness and saving time. The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Kusama and Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations.
