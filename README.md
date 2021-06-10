# Hot Cross Audits

This repository contains a public-facing list of audits that have been performed on the [Hot Cross](https://hotcross.com/) codebase and select Hot Cross products. We attempt to adhere to [Semantic Versioning](https://semver.org/) at all times but aren't anywhere near perfect in this regard. If multiple audits take place on the same codebase at the same time then we sometimes adjust versioning on the fly to accomodate for that. 

We have thus far conducted audits with [Beosin](https://lianantech.com/), [SlowMist](https://www.slowmist.com/), [Omniscia](https://omniscia.io/), [Zokyo](https://www.zokyo.io/), [CertiK](https://www.certik.org/), and [PeckShield](https://peckshield.com/en).

## [$HOTCROSS Token and Vesting](cross-token/)

### General Information

- Token Name: `Hot Cross Token`
- Token Symbol: `$HOTCROSS`
- Token Decimals: `18`
- Total Supply: `500,000,000`
- Initial Circulating Supply: `85,750,000` (The full token emission schedule is [here](http://hotcross.link/token).)
- ERC20 Contract Address: [0x4297394c20800E8a38A619A243E9BbE7681Ff24E](https://etherscan.io/address/0x4297394c20800e8a38a619a243e9bbe7681ff24e)
- BEP20 Contract Address: [0x4FA7163E153419E0E1064e418dd7A99314Ed27b6](https://bscscan.com/address/0x4FA7163E153419E0E1064e418dd7A99314Ed27b6)

### 1.0.1

- Omniscia: [Pass](https://omniscia.io/hot-cross-vesting-implementation/)

### [1.0.0](cross-token/1.0.0/)

- Beosin: [Pass](cross-token/1.0.0/Beosin%20Audit%20Report%20-%20Hot%20Cross%20Token%20V1.0.0.pdf)
- SlowMist: [Pass](cross-token/1.0.0/SlowMist%20Audit%20Report%20-%20Hot%20Cross%20Token%20V1.0.0.pdf)

## [Cross Bridge](cross-bridge/)

### [1.0.1](cross-bridge/1.0.1/)

- Beosin: [Pass](cross-bridge/1.0.1/Beosin%20Audit%20-%20Hot%20Cross%20BSC%20Bridge%20V1.0.1.pdf)
- SlowMist: [Pass](cross-bridge/1.0.1/SlowMist%20Audit%20Report%20-%20Hot%20Cross%20BSC%20Bridge%20V1.0.1.pdf)

### [1.0.0](cross-bridge/1.0.0/)

- Beosin: [Pass](cross-bridge/1.0.0/Beosin%20Audit%20-%20Hot%20Cross%20BSC%20Bridge%20V1.0.0.pdf)
- SlowMist: [Pass](cross-bridge/1.0.0/SlowMist%20Audit%20Report%20-%20Hot%20Cross%20BSC%20Bridge%20V1.0.0.pdf)

## [Cross Pool](cross-pool/)

💡 TLDR: Cross Pool V1 is a "[launchpool](https://www.binance.com/en/blog/421499824684900950/Everything-You-Need-to-Know-About-Binance-Launchpool-How-to-Farm-Tokens-Calculate-APY--More)" on [Binance Smart Chain](https://www.binance.org/en/smartChain) and by extension a launchpool that's compatible with ETH and most EVM networks. It introduces features that we want, not only to launch `$HOTCROSS` to market but also to allow for other teams in the space to participate in LP staking and single-sided staking without having to reinvent the wheel on-chain as we've done. 

In the first iteration of Cross Pool, which has been rigorously [audited](cross-pool/1.0.5/), we support: **a) rewards pools with multiple LP token staking pools, b) rewards pools with single-sided staking pools, c) rewards pools with a mix of both, and d) delayed pools that reward users but only after a certain amount of time has passed.** We're stoked to be launching this on mainnet in the coming days and also distributing a large portion of `$HOTCROSS` on it.

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

## [Cross Mint](cross-mint/)

### [1.0.0](cross-mint/1.0.0/)

- Beosin: [Pass](cross-mint/1.0.0/Beosin%20Audit%20-%20Cross%20Mint%20V1.0.0.pdf)
