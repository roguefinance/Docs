---
description: Detailing Maverick's voting system, introducing 'Ballot' and 'Bounty'.
---

# 🗳 Vote market

The Maverick system allows **veMAV** holders to vote in order to direct **MAV** inflation. They can direct emissions into each of the supported [Boosted Positions](../case-study/maverick-amm/boosted-positions.md).&#x20;

### Introducing Ballot

Ballot is a vote module where **eROG** holders can vote with a share of Rogue's **veMAV** voting power.

On Rogue, **MAV** lockers give up a % of their voting power to the protocol. This loss is compensated by the liquidity of the position, allowing lockers to exit their position if needed, plus a whole set of [rewards](rogue-for-mav-lockers.md).

### Introducing Bounty

Bounty is an incentives module where **eROG** holders can receive compensation from protocols interested in directing **veMAV**'s voting power. Protocols can provide Bounties for **eROG** holders to vote for a particular [Boosted Position](../case-study/maverick-amm/boosted-positions.md). **eROG** holders can consult current bounties, vote for a Boosted Position then collect the Bounties in addition to their usual [rewards](../tokenomics/incentives/revenue-sharing.md).

{% hint style="info" %}
Ballots can only accept bounties of whitelisted ERC20 tokens.
{% endhint %}

Voters can also delegate their **eROG** to anyone or to Rogue Protocol itself. This allows users to accumulate rewards without the cost of having to vote every 2 weeks on-chain.

{% hint style="success" %}
_On-chain Voting_

* _On-chain voting means that the votes are always transparent and auditable_
* _It also makes possible to use composability and automation on top by exposing voting data to anyone on the blockchain_
{% endhint %}

{% hint style="success" %}
_Flexibility_

* _Bounties parameters can be updated on-the-fly_
* _Vote incentivizers can also choose the ending time in advance, to avoid having to top up voting incentivizes weekly_
* _Voters are free to choose from many different protocols, offering a variety of voting incentivizes to engage with and vote on_
{% endhint %}

{% hint style="success" %}
_Incentive efficiency_

* _Vote incentivizers can set a maximum price per reward to avoid inefficient voting incentivizes_
* _Boosted Positions are flexible enough to make sure that they can only incentivize the expected behavior inside the pool._
{% endhint %}
