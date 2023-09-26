---
description: Explains Maverick's Boosted Positions for liquidity providers.
---

# Boosted Positions

#### Position Creation and Differentiation

When a user contributes liquidity to a Maverick pool, they have several options to establish a specific position within that pool. Each position is characterized by a set of key variables: the token pair, fee tier, bin width, liquidity mode, and liquidity distribution. For instance, one position might be a single Mode Right bin of **USDC** in the **USDC**/**USDT** pool with a 1% fee and 1% width, while another could be twenty-one Mode Static bins including both **USDC** and **USDT** in the same pool. \
Maverick's AMM positions provide users with a high degree of control and flexibility in terms of liquidity provision.

#### Introduction to Boosted Positions

In order to incentivize LPs to provide assets in a pool, anyone can create a Boosted Position for a pool. A Boosted Position operates just like any other position, with three significant distinctions:

* Boosted-Positions are incentivized across particular price ranges or for specific modes chosen by protocols.&#x20;
* Other users can contribute liquidity to a Boosted Position, effectively purchasing a share in that position.&#x20;
* Boosted Positions can be incentivized with additional token rewards, which are distributed among LPs who add liquidity to that Boosted Position.
* Boosted position are eligible to **MAV** liquidity mining

In other words, users can deposit more incentive tokens into the Maverick smart contract, which will then be distributed to LPs who own liquidity in a specific Boosted Position. These incentives act like enticements for other users to contribute more liquidity to that Boosted Position.

#### Liquidity Attraction with Boosted Positions

Protocols can channel incentives to a specific Boosted Position, offering a high degree of precision hence efficiency in their incentives. This introduces a new concept for protocols: _**incentive efficiency**._

{% hint style="success" %}
_**incentive efficiency:** optimizing the efficiency of an incentive program with the least capital requirement._
{% endhint %}

{% hint style="info" %}
_Example_

* _The **XYZ** project is looking to bootstrap liquidity for their token. They don't need LPs to bring more **XYZ** to Maverick: their treasury already has plenty of it._
* _What they need from users is a quote asset (e.g., **ETH**) that can be swapped against their **XYZ**. They could create a Boosted Position consisting only of **ETH** in an **XYZ**/**ETH** pool and then add incentives to the Boosted Position. This would encourage new LPs to add only **ETH** to the pool, effectively allowing project **XYZ** to rent only the liquidity they need for their pool._
{% endhint %}

[Learn more](https://docs.mav.xyz/guides/incentives/understanding-boosted-positions) on Maverick AMM's Boosted-Positions.

#### Alignment

In order to create effective incentives for liquidity providers, it's imperative to align the distribution of **MAV** emissions with the interests of the community. \
Maverick introduces a voting system which allows **MAV** holders to directly influence the distribution of **MAV** emissions, ensuring that the rewards are channeled towards the most useful pools. This democratic approach aims to align the interests of the community with the overall success of the protocol.

Learn about Maverick's voting system in the [next section](vemav.md#understanding-the-ve-governance).

