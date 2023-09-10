---
description: Details Maverick's AMM enhancements for improved DeFi interactions.
---

# Enhancements

#### Provision basics

Liquidity providers (LPs) play a crucial role in the Maverick Protocol by supplying liquidity to a pool, in which traders can execute swaps. As a reward for their contribution, LPs receive trading fees from each swap executed by traders.

#### Pool Composition and Liquidity Distribution

Each pool within the Maverick system comprises two tokens. Typically, an LP contributes equal quantities of both tokens, although there are instances where they might supply just one, a strategy often referred to as "single-sided liquidity". The actual ratio of the tokens is determined by the distribution selected by the LP.

The Maverick Protocol employs a unique system of [non-uniform liquidity distribution across bins](https://docs.mav.xyz/guides/liquidity-providers/understanding-modes) allowing for granular on-chain market-making strategies, while keeping gas costs at a minimum.

At any given moment, only one bin in a pool is active, meaning swaps are actively happening at that price point using the liquidity in that bin. As the token ratio in the pool shifts, the price moves to a new bin, which then becomes the active bin. LPs collect fees only when their liquidity is in the currently active bin.

#### Pool Deployment and Fees

When a pool is initially deployed on Maverick, the deploying LP selects a fee tier in addition to the bin width. This fee tier determines the percentage of the swap value a trader will be charged when swapping with the pool.

From an LP's perspective, it's possible to deploy multiple pools for the same pair, each with different fee tiers and widths. Traders, on the other hand, don't choose between pools. They decide the amount they want to swap, and the AMM intelligently routes their swap to the pool offering the best value at that moment. This might sometimes mean paying a higher fee for a better price. The market ultimately determines the optimal fee tier and width for each token pair.

[Learn more](https://docs.mav.xyz/guides/liquidity-providers/how-to-add-liquidity) on how to add liquidity.

LPs earn fees based on their pro rata share of the current active bin. These fees are auto-compounded back into the pool, allowing the LP's position in the pool to grow proportionally. When an LP exits their position, they redeem their proportional share from the bins in which they are staked.

#### Liquidity Modes in Maverick AMM

The Maverick AMM offers four pre-configured liquidity modes:

1. Mode Right
2. Mode Left
3. Mode Both
4. Mode Static

Each mode is designed to support a specific type of liquidity strategy. The first three modes leverage Maverick AMM's intelligent liquidity-shifting technology to keep your liquidity active within certain parameters. All liquidity shifting is performed natively by the Maverick AMM smart contract, eliminating the need for LPs to pay gas to move their liquidity.

[Learn more](https://docs.mav.xyz/guides/liquidity-providers/the-basics) on Maverick AMM's liquidity provision.
