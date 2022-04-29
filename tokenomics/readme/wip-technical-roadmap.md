---
description: A tentative technical roadmap for Discoin. Subject to frequent revisions.
cover: >-
  https://images.unsplash.com/photo-1471958680802-1345a694ba6d?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxOTcwMjR8MHwxfHNlYXJjaHwzfHxyb2FkbWFwfGVufDB8fHx8MTY1MTI0NzE0Mw&ixlib=rb-1.2.1&q=85
coverY: 0
---

# 🏗 \[WIP] Technical Roadmap

{% hint style="warning" %}
This Technical Roadmap is a work-in-progress. We'll be updating it frequently as work begins and more concrete details become available.
{% endhint %}

We propose to begin with a pragmatic, effective approach where necessary, and to gradually and iteratively replace trustful solutions (multisigs) with trustless tooling (smart contract governance) where it would be logical to implement.

As we work with our technical partners, we will revise this document, adding different tooling details or specifications and projected delivery dates.

### Bounties

We propose to fund bounties for the different development tasks outlined here in both the near-term plan and the long-term plan.

You can find the items we propose to bounty / fund marked with `#bounty` below.\


### Phase 1

#### Multisigs

A number of Discoin committees will be formed to steward the proper distribution schedule of Discoin.  These committees will be bound to act on the multisig in accordance with the Discoin Litepaper. \
\
Be aware that the Discoin committees will hold the funds in trust for distribution. They will be effectively frozen until distribution / inflation events. The funds will not be available for spending for any reason until they are released by inflation into the respective Governance wallets, which will be created and used at the first distribution epoch for that fund.

For example, the funds in the Discoin Community Fund Committee multisig will keep the funds frozen in the committee wallet until the first distribution event, where the funds will be airdropped to the wallet of the governance structure that will control the purse strings for the Community Fund in accordance with whatever community governance protocol is established for that purpose.

Note that during Genesis the Treasury multisig receives an airdrop -- this is a governance wallet, so from the Genesis event there will be funds that need to be governed by the community.

#### Fractionalization of Charles

* via Fracada v2 from dcSpark
* 5,777,777,777 to Originating Address #multisig

#### Genesis

* outputs
  * \[\[Treasury]] #multisig receives Airdrop
    * 333,777,729 Discoin
  * \[\[Airdrop]] Script #bounty
    * 333,777,729 Discoin
    * Identify all wallets holding Discos
    * Blacklist jpg.store wallets
    * For each wallet
      * Count Discos per wallet
      * Disperse 57777 per Disco in one tx
      * Remove Discos from unclaimed pool
    * Send Unclaimed Pool (5777 funds remainder) to \[\[Community Pool]] #multisig
  * To be frozen for future distribution
    * \[\[LP]] Committee #multisig - 25% of future inflation --&#x20;
    * \[\[Community Pool]] Committee #multisig - 25% of future inflation
* \[\[Originating Address]] will begin functioning as the \[\[Staking]] Committee #multisig with remaining funds (50% of future inflation)

#### Staking Rewards

* script (v1) #bounty
  * Define epoch
  * Method
    * 1 Disco PFP required to stake
      * Commit Discoin to be staked against PFP NFT to smart contract
      * Must unstake via original PFP NFT
      * Must unstake before end of epoch to withdraw after beginning of next epoch
      * Rewards compound if staked epoch to epoch
* smart contract (v2) #bounty

#### Governance / Voting

* \#bounty
  * Gather votes on arbitrary measures in decentralized, verifiable manner based on PFP in wallet

### Phase 2

#### Governance

* \[\[Voting]]
  * phase 1
    * Catalyst-like fund management and voting infrastructure #bounty
    * Votes bind on smart contract action in verifiable / transparent way where funds / proposals are concerned
    * \[\[Proposals]] #bounty
      * \[\[Treasury]]
      * \[\[Community Pool]]
  * phase 2
    * \[\[Constitutional Amendments]]
    * \[\[Elections]]
      * Committees / Governing Bodies
      * Governance Initiatives
    * \[\[Jury]] decisions for dispute resolutions \[\[Court]] in the \[\[Commons]]
