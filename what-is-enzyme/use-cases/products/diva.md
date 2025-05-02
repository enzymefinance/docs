---
description: >-
  Diva vaults were launched on Enzyme as a way to accelerate pre-launch TVL.
  More information can be found on the official Diva page diva.enzyme.finance.  
  Below are some FAQ.
cover: ../../../.gitbook/assets/Diva-Cover.png
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Diva

### Where can I find the official T\&Cs for the Early Stakers Initiative?

The official reference is [DIP-02](https://www.tally.xyz/gov/diva/proposal/45468458207916765916984557235161596151150976178275597160417224501662414206717), which was voted and approved by the DAO.

### Can I deposit by sending assets directly to the vault address?

No. Deposits shall be made following the Enzyme UI without sending funds directly to the vault address. Funds sent directly to the address would not mint new vault shares for the depositor so the value would be "airdropped" to the current shareholders and therefore lost by the depositor.&#x20;

<figure><img src="https://lh4.googleusercontent.com/YY0OnXDbOds19lfsouwuwebklZ0XUoYcVmLT0v7CIhd5KTRUwwET-WY2NldZ9Ezk09wmtvfJIkqPu5hcpXo96e7e9Hkpn75DgLvDcZfbnW2RpbDKC2AQPsXaCLRoAgn3fjDxJvvVo-QAOjFDhXSmc48" alt=""><figcaption></figcaption></figure>

### Where can I send my questions if the FAQ does not cover my doubts or if I have a technical issue to troubleshoot?

You can send an email to diva@enzyme.finance. You’ll receive an answer within 24h. In case of technical issues, please consider adding the following details:&#x20;

* Wallet address used for deposit.
* Type of wallet (e.g., Metamask, Safe, Ledger).
* Connection method (e.g., via WalletConnect, Ledger through Metamask).
* Steps you took when the issue occurred.
* Any screenshots of the error you witnessed.

### Where can I follow the progress of the initiative in terms of TVL?&#x20;

You can see the TVL on the [stETH vault here](https://diva-steth.enzyme.community/vault/0x1ce8aafb51e79f6bdc0ef2ebd6fd34b00620f6db?currency=ETH)

You can see the TVL on the [ETH vault here](https://diva-eth.enzyme.community/vault/0x16770d642e882e1769ce4ac8612b8bc0601506fc?currency=ETH)

### I can’t sign the special T\&Cs with my Safe. How do I do it?

If your Safe is doing on-chain signatures, it will not work. You will need to do off-chain signatures. You should be able to change this in “Settings” -> “Safe Apps” -> “Signing Method”, which should be left unchecked. \


<figure><img src="https://lh3.googleusercontent.com/2M0vLyDpjQ3-ptO8-KjEpzNXlV2foOl58j7IyvKzFdc2W3PIO20aXbf3id2_i9Khvaf9aobcmcttVbUktn-lD5M6K30khUUPPGWrtPaFJZ5uEvpW_f093PptEixOSoKBP8qk67CBpyjAu0NsKPk4obc" alt=""><figcaption></figcaption></figure>

### Where/how do we see how much DIVA I have accrued so far?

As you can also see from the T\&Cs approved on [DIP-02](https://www.tally.xyz/gov/diva/proposal/45468458207916765916984557235161596151150976178275597160417224501662414206717), the accrual of DIVA won't start until 30 days prior to mainnet launch. Since that date is still to be determined, the accrual will be accounted as a 30-day lookback from the launch date. As the launch date approaches, we'll&#x20;

see how we can hook up our API with a dashboard that gives each staker a personalised overview of the DIVA accrued to date. Since rewards (i.e. DIVA/ETH/Day) are decreasing as TVL grows, today's deposits are useful to lock in the highest tier.&#x20;

### Why do I see ETH as an option for deposit on the stETH vault?

The stETH denominated vault accepts stETH deposits (kinda obvious) but also ETH deposits. In case someone comes with ETH, the protocol automatically converts ETH into the denomination asset during the deposit process, using Paraswap. In other words, you don't have to convert/mint stETH yourself and the asset that lands on the vault is always the denomination one. This is a standard of the Enzyme architecture across all vaults.

### Is there any difference between the 2 vaults in terms of DIVA rewards?

No. DIVA rewards will be the same for both vaults. The only difference is that the stETH vault will keep earning you staking rewards through the LST rebasing mechanism on top of DIVA incentives.&#x20;

### Why am I not getting 1:1 DSTVL vault shares with my stETH deposit?

That's because as time goes by the vault starts to accrue rebasing ETH staking rewards on the pre-existing AUM so the vault share DSTVL starts to appreciate relative to stETH in a non-rebasing manner. A good example of this is the Unslashed Finance [vault](https://app.enzyme.finance/vault/0x86fb84e92c1eedc245987d28a42e123202bd6701?currency=ETH), where you can see the share appreciation over time as a result of stETH rewards.

### What is the handover from Avantgarde Treasury to Diva DAO?

The handover refers to the moment when the ownership of the Enzyme vaults is transferred from Avantgarde Treasury to Diva DAO. Enzyme is a non-custodial fund management protocol where owning a vault doesn’t imply owning the funds within it.

### Can anyone access the funds within the Diva vaults on Enzyme?

No, the Diva vaults on Enzyme operate on a non-custodial basis, meaning that only the stakers, who have received vault shares upon their deposit, can access the funds. There are no custodians involved in this setup.

### What security measures are in place for configuration changes to the vaults?

Currently, a 2/4 signature is needed for any change to the vault configuration, soon transitioning to a 3/5 consensus. Additionally, a 7-day timelock is triggered in the event of a configuration change, allowing stakers to redeem their assets in case the change is unauthorized before it takes effect.

### What is the significance of transferring ownership to the DAO?

Once ownership transition is completed, any modifications will require an on-chain DAO vote, extending the notice window for all stakeholders, thereby enhancing security and stakeholder involvement.

### Why has the handover to Diva DAO not taken place yet?

The handover has not occurred yet to avoid potential UX/UI frustrations and delays in implementation. Concerns include the current clunky UI/UX for changing granular vault settings from Tally and the necessity for vault reconfiguration to add connectivity to Lido native redemption and to Diva’s staking/divETH minting.

### What actions are planned to improve the setup before and during the handover?

In the short term, the plan involves increasing the signature threshold of Avantgarde Treasury's multisig to 3/5 signers and arranging a technical AMA with Enzyme’s auditor. In the medium term, the plan includes accelerating conversations with Tally & Aragon regarding the adjustment of granular vault settings following a successful on-chain DAO vote, defining a clear ETA for secure implementation and ownership transfer, and proposing and voting on the handover of vault ownership to Diva DAO

### How does the multisig security work and what is the planned transition regarding signature consensus?

The multisig security requires a specific number of signatures (2/4 initially, transitioning to 3/5) for any change to the vault configuration, ensuring that no single entity can make unilateral changes and enhancing the overall security of the vaults.

### What can stakers do in the event of an unauthorized configuration change?

If an any configuration change occurs, a 7-day timelock is initiated. Stakers can use this window to redeem their assets before the changes are implemented, ensuring they retain control over their holdings.

### Where can more detailed information be found regarding the upgrade and architectural design of the Enzyme's infrastructure?

\
More information on signalling an upgrade and the overall architectural design can be found here: \


* [https://docs.enzyme.finance/managers/signal-an-upgrade](https://docs.enzyme.finance/managers/signal-an-upgrade)
* [https://medium.com/enzymefinance/fund-in-the-shell-e82c46a0a0fa](https://medium.com/enzymefinance/fund-in-the-shell-e82c46a0a0fa)

### How committed is Avantgarde Treasury to transferring ownership to the DAO and what is the intended impact?

Avantgarde Treasury is fully committed to transferring ownership to the DAO. The completion of this transition means that any future modifications will necessitate an on-chain DAO vote, thereby extending the notice window for all stakeholders and enhancing democratic decision-making processes.

\
\
\


\
\


\
\
\
\
