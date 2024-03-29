---
description: 'Setup: Step 6 (Asset Management settings can be changed after creation)'
---

# Asset Management

Vault Managers can specify policies that restrict the behaviour in a vault to reassure stakeholders.&#x20;

![](<../../.gitbook/assets/Asset Managment.png>)

## **Limit Adapters To A Specific List**

Adapters connect your vault to DeFi protocols that allow you to trade, lend, borrow, supply liquidity, Stake, etcetera. Enebling this policy means that your vault will only be able to interact with adapters on this list.&#x20;

## Limit External Positions To A Specified List

An external position type is a new type of position which has been introduced with Sulu. They are similar to adapters in that they allow you to interact with external DeFi protocols. However, they differ in that they are not represented by a liquid, divisible, fungible token (eg. Compound CDPs or Uniswap v3 LP positions, Maple Lending, Aave Borrowing and Convex Voting). This policy defines which external position “types” can the vault interact with. [See risks & nuances section](https://userdocs.enzyme.finance/risks). Enabling this policy means that your vault will only be able to interact with external positions on this list.&#x20;

## **Set Cumulative Slippage Tolerance**

This policy is designed to limit any maliciously deliberate attempts or accidental actions which could drain a vault causing a large loss.&#x20;

It does this by limiting the value loss (i.e. slippage) that can occur via adapter actions over a “tolerance period” (rolling 7 day period).&#x20;

Vaults define a tolerance threshold (e.g., 5%, 10%, etc). Whenever an adapter action results in slippage, that slippage amount is added to a cumulative slippage total. The accumulated slippage then diminishes over the “tolerance period duration” at a constant rate based on the fund’s chosen tolerance. This policy allows bypassing the slippage checks entirely if the adapter being called is in a Council-maintained list on the AddressListRegistry (adapters that cannot be manipulated by asset managers to steal fund value).&#x20;

## Restrict External Position Removal

Prevents the removal of an external position from the vault’s accounting unless its value can be considered negligible (i.e. dust). The dust threshold is maintained by the Enzyme Council.&#x20;

## Restrict Asset Position Removal

Prevents the removal of an external position from the vault's accounting unless a) it does not have a valid price, or b) its value can be considered negligible (i.e. dust). The dust threshold is maintained by the Enzyme Council.
