# Safe - Ethereum

### **Step 1: Connect to Enzyme with a multisig.** <a href="#id-7f3a" id="id-7f3a"></a>

If you don’t already have a multisig safe, go to the [Safe app](https://app.safe.global/welcome) and follow the instructions to set up your Safe. If you already have one ready, just load it up from the app.

Once you’re set up with your Safe, click on Apps -> Wallet Connect.

![](https://miro.medium.com/max/3200/0\*z95AhyUinRM09Fci)

Now go to the [Enzyme App](http://app.enzyme.finance/) and connect using Wallet Connect. You’ll see a QR code pop up which you need to copy to clipboard. Now go back to the Safe page and paste the QR code into the wallet connect box highlighted in the image above.

You’re now connected to Enzyme with your multisig!

### **Step 2: Setting up with Enzyme.** <a href="#id-7fae" id="id-7fae"></a>

If you go back to the [Enzyme app](http://app.enzyme.finance/) now, you’ll see you are connected with your multisig wallet! You can now start plugging your organisation into Enzyme. Make sure you are on the “For Vault Managers” launchpad and click “Create”. If in doubt, you can refer to our [user docs](http://userdocs.enzyme.finance/) here or [contact us](https://t.me/enzymefinance).

### **Step 3: Deploying your Enzyme vault** <a href="#bba8" id="bba8"></a>

Once you’re done creating your organisation’s connection to Enzyme, you will get prompted to sign a transaction. Submit the transaction and then go back to the Safe App. Make sure you are logged in with one of the **multisig** **Owner** addresses and connect with Wallet Connect. It should prompt you to sign a transaction. Now keep repeating this process with other **multisig Owners** until you’ve passed the signing threshold. At that point, your Enzyme vault should be deployed on-chain and visible on the Vault Manager launchpad. For more information on what you can do with Enzyme, this might be a good time to [refer our user docs](http://userdocs.enzyme.finance/).

### Recommendations

Safe Approval transactions take time and depending on how you have set up your safe wallet, you may need additional extra steps. It can be slow and inefficient to pass the multisig threshold every time you need to do a trade or interact with a DeFi protocol on Enzyme. So we’ve come up with a way to delegate trading to one address. The owner of this address can be a bot, a company’s trader or an assigned group delegated by a DAO.

In order to delegate trading to one (or more) addresses, go to the Settings tab from the Vault Manager Launchpad and scroll down until you see Delegate Trading. Enter the Ethereum address and the add user address and submit the transaction. Now just go back to the Safe app and repeat the steps provided earlier. Ask the multisig owners to log in with their address, connect via Wallet Connect and sign the pending transaction.



### I can’t sign the special T\&Cs with my Safe. How do I do it? <a href="#i-cant-sign-the-special-t-and-cs-with-my-safe.-how-do-i-do-it" id="i-cant-sign-the-special-t-and-cs-with-my-safe.-how-do-i-do-it"></a>

If your Safe is doing on-chain signatures, it will not work. You will need to do off-chain signatures. You should be able to change this in “Settings” -> “Safe Apps” -> “Signing Method”, which should be left unchecked.
