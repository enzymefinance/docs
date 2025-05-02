# Add Safe Wallet To Your Enzyme Account

_If you are not already using SAFE with Enzyme, pls skip to_ [_this_](../../general-info/vaults-for-organisations/) _page to find out how you can._

When you add a wallet to your account, you need to sign a message with that wallet to prove that you have control over that wallet.

Adding a Safe wallet to your Enzyme account is slightly more complicated, because signing a message with a Safe wallet is an actual transaction that needs to be sent to the blockchain.

Here are the detailed steps to add a Safe wallet to your Enzyme account:

1. **Sign up / Sign in** to your Enzyme account.
2. **Connect your safe wallet**, if you don't know how to do that you can check it in [here](https://docs.enzyme.finance/managers/vaults-for-organisations).
3. Go to your account profile and click on the "**Start Adding Wallet**" button.
4. A modal will appear where you need to click on the “**Sign with Wallet**” button.
5. **Check your Safe**, the transaction to sign the message should appear there. Click on the “**Submit**” button.
6. All the required number of wallets need to sign the proposed transaction in Safe, and the transaction then needs to be executed in Safe.
7. Once the transaction has been executed, you will need to copy some transaction details. C**opy the hash string of the** “**Sign Message \_data(bytes): 0x\[someLongHash]**”. (You would copy **0x\[someLongHash]**)
8. **Go back to the Enzyme App.** If the modal to start adding a safe wallet is still open ("**Start Adding Wallet**"), please close it.
9. Click on the “**Finish Adding Wallet**” button.
10. **Complete the modal** by adding a **wallet name**/label and **paste the hash string you copied in step 7 above** in the message hash field and click on the “**Submit**” button.

If you have problems with these steps, don't hesitate to reach out to [support@avantgarde.finance](mailto:support@avantgarde.finance).
