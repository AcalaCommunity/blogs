# **Acala เปิดตัว 'Acala EVM' สำหรับ DeFi บน Polkadot | ความเข้ากันได้ของ Ethereum กับฟังก์ชันของ Substrate แบบไม่จำกัด**

![Image for post](https://miro.medium.com/max/6000/1*FNYYia98MytjFEU1Dtuzqw.png)

## The Acala EVM leverages the best of Ethereum while unlocking Substrate’s full potential with a composable, single-wallet, Acala-EVM-Substrate-WASM experience with ‘bring your own gas’, on-chain auto-scheduling, and more.

Acala’s engineering team has custom-built and launched the Acala EVM! This innovation, novel to the Polkadot ecosystem, enables Acala to provide Solidity, Substrate, and Web3 developers a complete full-stack (Acala+EVM+Substrate+WASM) experience seamlessly with a single wallet. Acala EVM also brings protocol composability for EVM and Substrate runtime (aka pallets) and enables developers to build and deploy DApps on Acala with exceptional tooling support.

Just like Ethereum can do things Bitcoin will never be able to do, which subsequently inspired many new innovations, Substrate and Polkadot are categorically different from Ethereum in a way that will empower many new, chain-level innovations outside of the EVM sandbox. We are firm believers in the power of Substrate and built the Acala EVM to optimize for Substrate’s full potential and longevity, rather than simply redeploying Ethereum on Polkadot.

# **The Acala EVM**

## **Composable DeFi Environment**

Smart Contract Dapps deployed in Acala EVM can directly use native and cross-chain assets such as DOT, ACA, aUSD, renBTC, XBTC, and more. ERC-20 tokens deployed in the EVM can also be made available at the runtime level, to be listed in the DEX, or (by governance approval) to be used as gas fee tokens. This means that, for example, our friends at Ampleforth can deploy AMPL contracts on Acala EVM to be made available as a native token, so it can be used to pay transaction fees and listed directly on our DEX.

New to the concept of composability? A16z put it very well in their [4 Eras of Blockchain Computing: Degrees of Composability](https://a16z.com/2018/12/16/4-eras-of-blockchain-computing-degrees-of-composability/#:~:text=A%20platform%20is%20composable%20if,more%20rapid%20and%20compounding%20innovation.).

To make this a bit more ‘real’, watch below as Acala Co-Founder and CTO Bryan Chen recently demonstrates one use case of the Acala EVM when he deployed Uniswap onto Acala and executed a trade within 2 minutes:

## **Other Fully Composable DeFi Primitives in the Acala EVM**

- **Bring your own gas**: Power transactions with virtually any token — The native and cross-chain tokens integrated with Acala will be able to be used for paying gas. When live it could look like this: _Are you sending wrapped ETH to Acala to start playing in DeFi? Send your ETH to Acala via the bridge, and start deploying your wrapped ETH immediately in the Acala DeFi apps using your wrapped ETH as the gas fee. No need to go out and find ACA._
- **On-chain automatic scheduler** that enables use cases like subscriptions and recurring payments. Try it [here](https://wiki.acala.network/build/development-guide/smart-contracts/advanced/use-on-chain-scheduler) or watch the 6 min demo below.

- **Native and cross-chain tokens** available in ERC20: DOT, ACA, aUSD, XBTC (from ChainX), LDOT (liquid staking DOT), RENBTC, and more
- Network of oracles to get price feeds. Try it [here](https://wiki.acala.network/build/development-guide/smart-contracts/advanced/use-oracle-feeds).
- Protocols such as DEX, stablecoin lending, and liquid staking derivatives (e.g. liquid DOT for your staked DOT)

## **🐰🕳 For a deep dive on the Acala EVM, check out the** [**Acala Wiki’s in-depth EVM section**](https://wiki.acala.network/learn/basics/acala-evm/acala-evm-composable-defi-stack)**.**

## Try it out at ETHDenver 2021

Acala is debuting the Acala EVM at ETHDenver 2021, offering $3k USD for hackers to “**Build a DApp Using the Acala EVM**” or “**Build a DApp Using the Acala EVM with the On-Chain Automatic Scheduler Function**”.

- Find Acala’s [**ETHDenver Hacker guide**](https://wiki.acala.network/general/contribution-rewards/ethdenver-hacker)**.**
- Check out [**ETHDenver’s Bounty Hub**](https://www.ethdenver.com/post/acala) and [**Team Guidelines**](https://www.ethdenver.com/judging)**.**

[Make Your DeFi DApp Polkadot-Ready with Acala’s EVM at ETHDenver 2021](https://medium.com/acalanetwork/make-your-defi-dapp-polkadot-ready-with-acalas-evm-at-ethdenver-2021-b542090f6af1)

# **Acala at a High Level**

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
