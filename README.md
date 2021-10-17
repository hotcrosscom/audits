# Hot Cross Audits

This repository contains a public-facing list of audits that have been performed on the [Hot Cross](https://hotcross.com/) codebase and select Hot Cross products. We attempt to adhere to [Semantic Versioning](https://semver.org/) at all times but aren't anywhere near perfect in this regard. If multiple audits take place on the same codebase at the same time then we sometimes adjust versioning on the fly to accomodate for that. 

We have thus far conducted audits with [Beosin](https://lianantech.com/), [SlowMist](https://www.slowmist.com/), [Omniscia](https://omniscia.io/), [Zokyo](https://www.zokyo.io/), [CertiK](https://www.certik.org/), and [PeckShield](https://peckshield.com/en).

## [Hot Cross Token and Vesting](cross-token/)

### General Information

- Token Name: `Hot Cross Token`
- Token Symbol: `$HOTCROSS`
- Token Decimals: `18`
- Total Supply: `500,000,000`
- Initial Circulating Supply: `85,750,000` (The full token emission schedule is [here](https://hotcross.link/hotcross-economy).)
- Current Supply: https://api.hotcross.com/supply
- [Ethereum](https://ethereum.org/) Contract Address: [0x4297394c20800E8a38A619A243E9BbE7681Ff24E](https://etherscan.io/address/0x4297394c20800e8a38a619a243e9bbe7681ff24e) (Canonical)
- [Binance Smart Chain](https://www.binance.org/en/smartChain) Contract Address: [0x4FA7163E153419E0E1064e418dd7A99314Ed27b6](https://bscscan.com/address/0x4FA7163E153419E0E1064e418dd7A99314Ed27b6) (Bridge) ([link](https://bridge.hotcross.com/))
- [Avalanche C-Chain](https://www.avax.network/) Contract Address: [0x2f86508f41310D8D974B76deb3D246c0caa71cf5](https://cchain.explorer.avax.network/tokens/0x2f86508f41310D8D974B76deb3D246c0caa71cf5/token-transfers) (Bridge) ([link](https://bridge.hotcross.com/))
- [Polygon](https://polygon.technology/) Contract Address: [0x3b737a181f7d2532cF49864f8050b3465a310593](https://polygonscan.com/token/0x3b737a181f7d2532cF49864f8050b3465a310593) (3rd-Party Mapped) ([link](https://mapper.matic.today/))
- [Harmony](https://www.harmony.one/) Contract Address: [one1u0tuw46yh9m09kkxs7znwjtwwhm754h3lp0jzn](https://explorer.harmony.one/address/0xe3d7c75744b976f2dac6878537496e75f7ea56f1) (3rd-Party Bridge) ([link](https://bridge.harmony.one/))

Canonical (and thus its audits) resides on Ethereum. The Binance Smart Chain BEP20 is an ever-fluctuating supply that relies on the inflow and outflow of [Cross Bridge](https://bridge.hotcross.com/), and 3rd-party mapped assets rely on those bridge technologies.

### [1.0.2](cross-token/1.0.2/)

- Beosin: [Pass](cross-token/1.0.2/Beosin%20Audit%20Report%20-%20Hot%20Cross%20Token%20V1.0.2.pdf)
- SlowMist: [Pass](cross-token/1.0.2/SlowMist%20Audit%20Report%20-%20Hot%20Cross%20Token%20V1.0.2.pdf)

### [1.0.1](cross-token/1.0.1/)

- Omniscia: [Pass](https://omniscia.io/hot-cross-vesting-implementation/)

### [1.0.0](cross-token/1.0.0/)

- Beosin: [Pass](cross-token/1.0.0/Beosin%20Audit%20Report%20-%20Hot%20Cross%20Token%20V1.0.0.pdf)
- SlowMist: [Pass](cross-token/1.0.0/SlowMist%20Audit%20Report%20-%20Hot%20Cross%20Token%20V1.0.0.pdf)

---

## [Cross Bridge](cross-bridge/)

💡 Note that this is now live on mainnet at [bridge.hotcross.com](https://bridge.hotcross.com/).

### [1.0.1](cross-bridge/1.0.1/)

- Beosin: [Pass](cross-bridge/1.0.1/Beosin%20Audit%20-%20Hot%20Cross%20BSC%20Bridge%20V1.0.1.pdf)
- SlowMist: [Pass](cross-bridge/1.0.1/SlowMist%20Audit%20Report%20-%20Hot%20Cross%20BSC%20Bridge%20V1.0.1.pdf)

### [1.0.0](cross-bridge/1.0.0/)

- Beosin: [Pass](cross-bridge/1.0.0/Beosin%20Audit%20-%20Hot%20Cross%20BSC%20Bridge%20V1.0.0.pdf)
- SlowMist: [Pass](cross-bridge/1.0.0/SlowMist%20Audit%20Report%20-%20Hot%20Cross%20BSC%20Bridge%20V1.0.0.pdf)

---

## [Cross Pool](cross-pool/)

💡 TLDR: [Cross Pool](https://crosspool.hotcross.com/) V1 is a "[launchpool](https://www.binance.com/en/blog/421499824684900950/Everything-You-Need-to-Know-About-Binance-Launchpool-How-to-Farm-Tokens-Calculate-APY--More)" on [Binance Smart Chain](https://www.binance.org/en/smartChain) and by extension a launchpool that's compatible with ETH and most EVM networks. It introduces features that we want, not only to launch `$HOTCROSS` to market but also to allow for other teams in the space to participate in LP staking and single-sided staking without having to reinvent the wheel on-chain as we've done. 

In the first iteration of [Cross Pool](https://crosspool.hotcross.com/), which has been rigorously [audited](cross-pool/1.0.5/), we support: **a) rewards pools with multiple LP token staking pools, b) rewards pools with single-sided staking pools, c) rewards pools with a mix of both, and d) delayed pools that reward users but only after a certain amount of time has passed.** We're stoked to be launching this on mainnet in the coming days and also distributing a large portion of `$HOTCROSS` on it.

### [1.0.5](cross-pool/1.0.5/)

- PeckShield: [Pass](cross-pool/1.0.5/PeckShield%20Audit%20Report%20-%20Cross%20Pool%20V1.0.5.pdf)

### [1.0.3](cross-pool/1.0.3/) & [1.0.4](cross-pool/1.0.4/)

- CertiK: [Pass](cross-pool/1.0.4/CertiK%20Audit%20Report%20-%20Cross%20Pool%20V1.0.4.pdf)

### [1.0.2](cross-pool/1.0.2/)

- Omniscia: [Pass](https://omniscia.io/hot-cross-cross-pool/)
- Zokyo: [Pass](cross-pool/1.0.2/Zokyo%20Audit%20Report%20-%20Cross%20Pool%20V1.0.2.pdf)

### [1.0.0](cross-pool/1.0.0/) & [1.0.1](cross-pool/1.0.1/)

- Beosin: [Pass](cross-pool/1.0.0/Beosin%20Audit%20Report%20-%20Cross%20Pool%20V1.0.0.pdf)
- SlowMist: [Pass](cross-pool/1.0.0/SlowMist%20Audit%20Report%20-%20Cross%20Pool%20V1.0.0.pdf)

---

## [Cross Mint](cross-mint/)

💡 Cross Mint is a multi-chain 721/1155 NFT minter that allows creators and hobbyists to mint our their creations on Ethereum, Polygon, Binance Smart Chain, HECO, and KCC. This is now live on mainnet and available for use at [mint.hotcross.com](https://mint.hotcross.com/).

### Smart Contract Addresses ([BSC](https://bscscan.com/), [ETH](https://etherscan.io/), [MATIC](https://polygonscan.com/), [HECO](https://scan.hecochain.com/home/index), [KCC](https://explorer.kcc.io/en/))

```json
// Binance Smart Chain
{
  "crossMint721": "0x1316F7D656ea26Aa8141cb045329168b15E72186",
  "crossMint1155": "0x460f839F260E7e418dd7e4D8dEC811694a33b588"
}
// Ethereum
{
  "crossMint721": "0x096aD12B21DdF0EfdeC692532a0d1B42Fab59aEA",
  "crossMint1155": "0xC5Af3186829A38b06B8FD02c10683E9629A5Bbe7"
}
// Polygon
{
  "crossMint721": "0xd87a431067CAab669fF72ea4bCFd03A513D80bEd",
  "crossMint1155": "0x0C3d4dD9968c59302575d3D3E764c47180801057"
}
// Huobi ECO Chain
{
  "crossMint721": "0xDfb7CbE6a3e889216fFd84AA603453A1D6B40eBC",
  "crossMint1155": "0xF5E9FF9BfFeeA5d8AB13f7caE3f25e6A4083b808"
}
// KuCoin Community Chain
{
  "crossMint721": "0xe3a0c65cac05d952331cFEb87EdFE84B3799fc0B",
  "crossMint1155": "0xf912584A01797bfcE9F1029BE943458D30D170DB"
}
// Harmony
{
  "crossMint721": "0x0Ca40B486788d255607C343f7d221A08ef7e2634",
  "crossMint1155": "0x9F6870fEbe91D842f8602E2E594fa2D5C96a5637"
}
```

### [1.0.1](cross-mint/1.0.1/)

- SlowMist: [Pass](cross-mint/1.0.1/SlowMist%20Audit%20-%20Cross%20Mint%20V1.0.1.pdf)

### [1.0.0](cross-mint/1.0.0/)

- Omniscia: [Pass](https://omniscia.io/hotcross-crossmint-nft-implementation/)
- Beosin: [Pass](cross-mint/1.0.0/Beosin%20Audit%20-%20Cross%20Mint%20V1.0.0.pdf)

---

## [Cross Send](cross-send/)

### [1.0.0](cross-send/1.0.0/)

- Omniscia: [Pass](https://omniscia.io/hot-cross-cross-send/)
- Beosin: [Pass](cross-send/1.0.0/Beosin%20Audit%20-%20Cross%20Send%20V1.0.0.pdf)

---

## [IHO](iho/)

### [1.0.0](iho/1.0.0/)

- Beosin: [Pass](iho/1.0.0/Beosin%20Audit%20-%20IHO%20V1.0.0.pdf)

--- 

## [HOTVIP](hotvip/)

### [1.0.0](hotvip/1.0.0/)

- Omniscia: [Pass](https://omniscia.io/hot-cross-hotvip/)
- Beosin: [Pass](hotvip/1.0.0/Beosin%20Audit%20-%20HOTVIP%20V1.0.0.pdf)

---

## [Cross Yield](cross-yield/)

### [1.0.0](cross-yield/1.0.0/)

- Omniscia: [Pass](https://omniscia.io/hot-cross-cross-yield)
- Beosin: [Pass](cross-yield/1.0.0/Beosin%20Audit%20Report%20-%20Cross%20Yield%20V1.0.0.pdf)

---

## [KYC](cross-kyc/)

🔑 These smart contracts implement functions that allow users to [register and modify their email information](https://app.hotcross.com/kyc) for compliant products like IHO's and Launchpads. Users only need to pay a one-time fee to the charging address when registering and will always have access to Hot Cross products that require compliance. The owner of the smart contracts can only modify the fee and the fee receiving address. These fees are secured in a [Gnosis Safe](https://gnosis-safe.io/).

### [1.0.0](cross-kyc/1.0.0/)

- Beosin: [Pass](cross-kyc/1.0.0/Beosin%20Audit%20-%20Hot%20Cross%20KYC%20V1.0.0.pdf)
- CertiK: [Pass](cross-kyc/1.0.0/CertiK%20Audit%20-%20Hot%20Cross%20KYC%20V1.0.0.pdf)
