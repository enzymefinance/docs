# Safe - Polygon

1. Go to [app.enzyme.finance](https://app.enzyme.finance/).
2. On the top right corner, click on **Connect Wallet** and select **WalletConnect**.
3. Below the QR code, click on “Copy to clipboard”.
4. On a new browser tab, go to your [Safe Wallet](https://app.safe.global) account.
5. Navigate to **Apps** > **WalletConnect**.
6. **Paste the QR clipboard** you have previously copied at step 3 and make sure that it connects successfully to Enzyme.
7. **Go back to the Enzyme App**, you will see that your Safe wallet is now connected.
8. Now you can continue the process of [creating a vault](https://docs.enzyme.finance/managers/setup/vault-types). For an in-depth explainer of all decisions that you need to make creating a vault, you can watch this [video](https://www.youtube.com/watch?v=JfyjfA0pKas\&feature=youtu.be).
9. Once you have completed the vault creation process and you submit the transaction, a signature request will appear in your Safe.

{% hint style="info" %}
If you are using Ethereum mainnet, don’t click on Open Dapp, instead, click on “keep using WalletConnect”.
{% endhint %}

### Recommendations

Safe Approval transactions take time and depending on how you have set up your safe wallet, you may need additional extra steps. It can be slow and inefficient to pass the multisig threshold every time you need to do a trade or interact with a DeFi protocol on Enzyme. So we’ve come up with a way to delegate trading to one address. The owner of this address can be a bot, a company’s trader or an assigned group delegated by a DAO.

In order to delegate trading to one (or more) addresses, go to the Settings tab from the Vault Manager Launchpad and scroll down until you see Delegate Trading. Enter the Ethereum address and the add user address and submit the transaction. Now just go back to the Safe app and repeat the steps provided earlier. Ask the multisig owners to log in with their address, connect via Wallet Connect and sign the pending transaction.



### I can’t sign the special T\&Cs with my Safe. How do I do it? <a href="#i-cant-sign-the-special-t-and-cs-with-my-safe.-how-do-i-do-it" id="i-cant-sign-the-special-t-and-cs-with-my-safe.-how-do-i-do-it"></a>

If your Safe is doing on-chain signatures, it will not work. You will need to do off-chain signatures. You should be able to change this in “Settings” -> “Safe Apps” -> “Signing Method”, which should be left unchecked.
