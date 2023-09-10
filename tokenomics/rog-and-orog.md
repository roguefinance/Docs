---
description: Detailing ROG and introducing oROG, a solution to liquidity mining challenges.
---

# ROG & oROG

### ROG

_**ROG** is Rogue's native token._&#x20;

The **ROG** token is the Rogue Protocol native token. It is designed to add value to the Rogue ecosystem by allowing holders to lock it and acquire voting power over Maverick's emissions. It is emitted every week to a whole set of market participants aligned with the values and success of Rogue:

* [**rMAV**](../stake/rogue-for-mav-lockers/rmav.md) stakers
* [**bpVaults**](../stake/rogue-for-maverick-amm-lps/bpvaults.md) stakers
* **rMAV**/**MAV** LPs on Maverick
* **ROG**/**ETH** LPs on Maverick

#### Inflation schedule <a href="#inflation" id="inflation"></a>

Initially, the minting of **ROG** tokens will be done on a pro-rata basis in response to each **MAV** token claimed. At specific **MAV** issuance thresholds, the minting will be reduced, progressively vanishing until the max supply is eventually reached.

### oROG

#### Option Liquidity Mining

Traditional liquidity mining has revealed certain flaws that cannot be ignored. The presence of [liquidity locusts](https://andrecronje.medium.com/liquidity-mining-rewards-v2-50896e44f259) and opportunistic dumping poses challenges, leading to the rapid disappearance of liquidity and negative impacts on token prices. To address these issues, we introduce **oROG**, a call option token on **ROG**, as the incentive token for liquidity mining on the Rogue platform.

By utilizing call option tokens like **oROG** instead of vanilla tokens, Rogue overcomes the "something for nothing" problem inherent in liquidity mining. Liquidity providers are no longer simply receiving rewards for free; they gain the right to purchase **ROG** at a discounted price until option expiry.

{% hint style="info" %}
_Example 1: In the money (ITM)_

_Assume the price of ROG is 20 USDC, and the current discount is 50% less than the market price. The protocol issues 1 oROG to a LP, who promptly exercises the option and purchases 1 ROG for 10 USDC to Rogue._ \
_The ROG can then be sold on a DEX (Maverick for example)._
{% endhint %}

_Let's examine the gains and losses in this situation:_

| Participants                | Traditional liquidity mining | OLM                      |
| --------------------------- | ---------------------------- | ------------------------ |
| Rogue                       | -1 **ROG**                   | -1 **ROG**, +10 **USDC** |
| Maverick LP staker (farmer) | +20 USDC                     | +10 USDC                 |
| ROG/USDC liquidity pool     | +1 ROG, - 20 USDC            | +1 ROG, -20 USDC         |

We can observe a non-negligible improvement in the protocol and the farmer payouts compared to traditional liquidity mining. LPs of the rewarded token have the same payout.

{% hint style="info" %}
_Example 2: Out of the money (OTM)_

_Assume as above that the price of ROG is 20 USDC, and the current discount is 50% less than the market price._ \
_Now a week later, because of opportunistic dumping the price of ROG is 10$. The protocol issues 1 oROG to a LP, who in this case will not exercise the option because it wouldn't net any profits ($10 - $10 = 0)._
{% endhint %}

_Let's examine the gains and losses in this situation:_

* Farmer : gets no ROG incentives
* Rogue : gives out no ROG, got liquidity and generated fees for free
* ROG/ETH LPs : benefit from no ROG dumping

{% hint style="success" %}
_Benefits:_

* _This also provides a floor price for **ROG** : in case **ROG** is below the discounted price at option expiry, the farmer is disincentivized to exercise their **oROG** call option and sell **ROG**._
* _**Incentives recycling** : unexercised **oROG** don't increase **ROG** supply**;**_\
  _they are reused for incentivizing liquidity in the future**,** hence allowing Rogue to reward platform usage for the longest term._
* _Rogue incentivizes platform usage in the right time : the discount applied to oROG is directly proportional to current platform usage._\
  _The lower the usage, the bigger the discount and inversely._
* _Quote tokens collected (i.e **USDC**) can be used to_ \
  _- Build POL (Protocol Owned Liquidity) on Maverick AMM on liquid asset like LSTs and stablecoins._\
  _- Share proceeds as revenue with **ROG** and **MAV** lockers in stablecoins._\
  _- Fund protocol developments._
{% endhint %}

#### Discount mechanisms

The _Usage-Driven Discount_ tailors the discount rate of **ROG** tokens according to the current platform activity responsively. As platform usage decreases, the discount intensifies, and vice versa, ensuring that incentives are always in harmony with platform health and activity responsively.

The _Dynamic Discount_ empowers the protocol administrators to manually adjust the discount rate on **ROG** tokens, especially during unpredictable market conditions or when there's an immediate need to stimulate platform activity.

By fine-tuning the discount rate, the protocol can strategically incentivize more liquidity providers to participate or maintain their position within the ecosystem.

\
