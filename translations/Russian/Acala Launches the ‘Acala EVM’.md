# **Acala запускает "Acala EVM" для DeFi на Polkadot | Совместимость Ethereum с неограниченной функциональностью Substrate**

![Image for post](https://miro.medium.com/max/6000/1*FNYYia98MytjFEU1Dtuzqw.png)

## Acala EVM перенимает лучшее из сети Ethereum, используя весь потенциал Substrate с помощью объединяемого единого кошелька, Acala-EVM-Substrate-WASM с функцией «принеси свой газ», «ончейн» автопланированием и многим другим.

Разработчики Acala запускают Acala EVM! Это нововведение для экосистемы Polkadot, позволяющее Acala предоставлять разработчикам Solidity, Substrate и Web3 полный набор функций (Acala + EVM + Substrate + WASM) с помощью единого кошелька. Также Acala EVM обеспечивает возможность компоновки протоколов для EVM и Substrate (также известной как паллеты) и позволяет разработчикам создавать и запускать DApps на Acala с исключительной поддержкой инструментов.

Многие инновации были вдохновлены примером сравнения Ethereum и Bitcoin: "цифровое золото" никогда не сможет располагать теми функциями, которыми в данный момент многие пользуют на "Эфире". Substrate и Polkadot кардинально отличаются от Ethereum тем, что расширяют возможности многих новых блокчейн-инноваций за пределами песочницы EVM. Мы безоговорочно верим в силу Substrate и создали Acala EVM для того, чтобы оптимизировать весь потенциал Substrate, а не просто повторно развернули Ethereum на Polkadot.

# **Acala EVM**

## **DeFi-среда**

Развернутые на новой EVM смарт-контракты могут напрямую использовать собственные и кросс-чейн активы на базе Polkadot, такие как: DOT, ACA, aUSD, renBTC, XBTC и другие. Токены на основе Ethereum (ERC-20) могут быть добавлены в листинг на децентрализованной бирже (DEX) или (после голосования) использованы для оплаты за газ. Это значит, что, например, наши друзья из Ampleforth могут развернуть контракты AMPL на Acala EVM, и при этом использовать собственный токен платформы для оплаты комиссий (газа) за транзакции и листинга непосредственно на Acala DEX.

В новинку концепция компоновки? A16z очень хорошо описали это в своей «Эре блокчейн-вычислений: степени компоновки».

Для наглядности, посмотрите ниже короткое видео, на котором соучредитель и технический директор Acala Bryan Chen демонстрирует один из вариантов использования Acala EVM, где он развернул Uniswap на Acala и сделал "свап" всего за 2 минуты:

## **Что ещё можно в Acala EVM:**

- Использование собственного газа: вы можете проводить транзакции практически с любым токеном - собственные и кросс-чейн токены, интегрированные с Acala, можно будет использовать для оплаты комиссий. На практике это выглядит следующим образом: вы отправляете WETH в Acala, чтобы начать использовать DeFi? Отправьте свой ETH в Acala через мост и сразу же начните применение вашего WETH в приложениях Acala DeFi, используя ваш  WETH в качестве платы за газ. Нет никакой необходимости менять ваши активы и покупать токены ACA.
- Он-чейновый автоматический планировщик, который включает такие варианты использования, как подписки и регулярные платежи. Более детально вы можете ознакомиться по ссылке или посмотреть короткое видео ниже.

- Собственные и кросс-чейн токены, доступные в ERC20: DOT, ACA, aUSD, XBTC (от ChainX), L-DOT (застейканый токен DOT), renBTC и др.
- Собственная сеть оракулов для получения цен в режиме реального времени. Более подробно можно ознакомиться по ссылке.
- Поддержка протоколов, таких как: DEX, кредитование стейблкоинов и ликвидные деривативы для ставок (например, L-DOT для вашего застейканого DOT).

## Чтобы более детально изучить Acala EVM, вы можете перейти по ссылке.

## ETHDenver 2021

Acala дебютирует с Acala EVM на ETHDenver 2021, предлагая хакерам $3 000 за «создание DApp с использованием Acala EVM» или «создание DApp с использованием Acala EVM с функцией автоматического планировщика в сети».

- Руководство для хакеров
- Баунти-программа и Руководство для команд

[Подготовьте свой DeFi DApp на Polkadot с помощью EVM Acala на ETHDenver 2021](https://medium.com/acalanetwork/make-your-defi-dapp-polkadot-ready-with-acalas-evm-at-ethdenver-2021-b542090f6af1)

# **Acala на высоком уровне**

If you’re new here, Acala is an Ethereum-compatible decentralized finance (DeFi) platform built for scale, leveraging Polkadot’s multi-chain network. Although Acala is a parachain providing layer 1 infrastructure, the Acala team has also built out an entire application layer on top of the parachain. Acala’s applications are built around a stable asset (aUSD) and offers end-user applications such as borrowing, lending, synthetic asset trading, and interest earning, all executed extremely fast with inexpensive gas fees. Developers can also leverage Acala as a platform on which to build their own applications.

The platform offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange. **Overall, Acala’s platform also offers:**

1.  **Micro Gas Fees** — Acala solves the gas fee problem for DeFi users, in combination with the ability to ‘bring your own gas’ as mentioned above
2.  **Staking derivative L-DOT** (Liquid DOT to release liquidity from staked DOT for use in Acala’s DeFi applications)
3.  **Stablecoin borrowing and lending** (DOT, Bitcoin and L-DOT used as primary collateral asset)
4.  **Earning yield and interest**
5.  Trading on **decentralized exchange** (DEX)
6.  On-chain **governance**
7.  On-chain **Treasury**
8.  Native network of **aggregated oracle price feeds**
9.  **On-chain sovereign wealth fund** to sustain the network’s future ([read more](https://medium.com/acalanetwork/building-a-decentralized-sovereign-wealth-fund-6a5a0ae995b1))
10. **Continuously upgrade with no forks**: Keep in mind that Acala can upgrade seamlessly with no forks. This means that the future is virtually limitless. Any new Substrate pallet (a product or feature in the form of a DeFi primitive or runtime) can smoothly integrate into Acala. It’s like getting an iPhone 12 that will auto-upgrade to a 13, 14, 15+ in the palm of your hand.

![Image for post](https://miro.medium.com/max/3200/0*iHVQdZllz1MxLwuy)

http://apps.acala.network

Thanks for checking out the new Acala EVM. We’ll continue to keep you updated on the progress of the Acala EVM, as well as further educational material on the different benefits it provides to the ecosystem. As always, you can find us on [Discord](https://discord.gg/vdbFVCH), [subscribe to our newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) for updates, or any of our channels below:

![Image for post](https://miro.medium.com/max/2402/0*BvF8sTfeQd4Sc71D.png)

# **About Acala**

[Acala](http://acala.network/) is the decentralized financial hub and stablecoin of Polkadot that makes it fast and easy to use or build financial applications, improving trading efficiency and saving time. The platform, operated by micro gas fees, offers a suite of financial primitives: a multi-collateralized stablecoin backed by cross-chain assets like Bitcoin, a trustless staking derivative, and a decentralized exchange to unleash liquidity and power financial innovations. Acala is the de facto open platform for finance applications to use smart contracts or built-in protocols with out-of-the-box cross-chain capabilities and robust security.

[Discord](https://discord.gg/vdbFVCH) | [Website](https://acala.network/) | [Twitter](https://twitter.com/AcalaNetwork) | [GitHub](https://github.com/AcalaNetwork/Acala) | [Acala Wiki](https://github.com/AcalaNetwork/Acala/wiki) | [Newsletter](https://share.hsforms.com/1X9RxkXk-R62I0VNbATaDXw4h8qc) | [All Channels](https://linktr.ee/acalanetwork)
