---
title: "How to prove a Monero (XMR) payment"
parent: Tutorials
---

# How to prove a Monero (XMR) payment

Monero is unique among cryptocurrencies because you need additional information to prove payments. In this tutorial, we describe the simplest way to prove a Monero (XMR) payment.

## Information you need

To prove a payment, you need ALL of the following:

* The Monero transaction ID
* The recipient's Monero address
* The unique transaction key

## Using Cake Wallet

If you are using Cake Wallet, simply open the app, go to your transaction history screen, then click on the transaction entry. Then click on "View Transaction on Monero.com".

[![Cake Wallet home screen](/images/tutorials-prove-payment-cakewallet-1.jpg){:width="32%"}](/images/tutorials-prove-payment-cakewallet-1.jpg)
[![Cake Wallet transactions screen](/images/tutorials-prove-payment-cakewallet-2.jpg){:width="32%"}](/images/tutorials-prove-payment-cakewallet-2.jpg)
[![Cake Wallet transactions details screen](/images/tutorials-prove-payment-cakewallet-3.jpg){:width="32%"}](/images/tutorials-prove-payment-cakewallet-3.jpg)

Click the "Prove payment" button. The website will prompt you to add the recipeint's address and the transaction key.

[![Monero.com explorer transaction details](/images/tutorials-prove-payment-monerocom-2.png)](/images/tutorials-prove-payment-monerocom-2.png)

Click to copy these from your Cake Wallet transaction details page, and paste them into the website. Then, click the "Prove payment" button.

[![Monero.com explorer prove payment](/images/tutorials-prove-payment-monerocom-4.png)](/images/tutorials-prove-payment-monerocom-4.png)

You will see a table that contains all the outputs in the transaction. If any of the relevant outputs are associated with the Monero address and transaction key that you provided earlier, you will see a positive value under "Amount transferred". A breakdown of which of the specifc Monero outputs were associated with the recipeint's address appears in a table underneath.

[![Monero.com explorer prove payment](/images/tutorials-prove-payment-monerocom-5.png)](/images/tutorials-prove-payment-monerocom-5.png)

Copy the website link by clicking on your web browser's address bar. You can give this link to the recipient as proof of payment. An example payment proof link is shown below:

> https://monero.com/payment/e02085d31a951663f1a93c6346f89d116bc9596fd7365ae0b44cb36bc6ab7b85/86bZHZtaaCSb1mAtMbE2xF339YDhoucZu3XDLUpAFJK3X1MA4yY3j8xVKNk2ySfw5AGY2knCAyis7Be7YLZ9cKbsNUKJQT1/b4e94e0030c727c374a51f4f4b8a3f74d9503338cc3a64028c918be9f8e6ec00/

## Using a different wallet

No matter what Monero wallet you are using, it's easy to provide a Monero payment using the Monero.com block explorer!

First, go to [Monero.com/explorer](https://monero.com/explorer). You will see a search box. Paste your Monero transaction ID in the search box, then click the "Search" button.

[![Monero.com explorer](/images/tutorials-prove-payment-monerocom-1.png)](/images/tutorials-prove-payment-monerocom-1.png)

If the transaction record exists, it will be displayed. Sometimes it takes up to 5 minutes after sending for your transaction to be fully propagated. If it has been more than 5 minutes and you still do not see your transaction, then it might not have been sent correctly.

Click the "Prove payment" button. The website will prompt you to add the recipient's address and the transaction key.

[![Monero.com explorer transaction details](/images/tutorials-prove-payment-monerocom-2.png)](/images/tutorials-prove-payment-monerocom-2.png)

Click to copy these from your Cake Wallet transaction details page, and paste them into the website. Then, click the "Prove payment" button.

[![Monero.com explorer prove payment](/images/tutorials-prove-payment-monerocom-4.png)](/images/tutorials-prove-payment-monerocom-4.png)

You will see a table that contains all the outputs in the transaction. If any of the relevant outputs are associated with the Monero address and transaction key that you provided earlier, you will see a positive value under "Amount transferred". A breakdown of which of the specifc Monero outputs were associated with the recipient's address appears in a table underneath.

[![Monero.com explorer prove payment](/images/tutorials-prove-payment-monerocom-5.png)](/images/tutorials-prove-payment-monerocom-5.png)

Copy the website link by clicking on your web browser's address bar. You can give this link to the recipient as proof of payment. An example payment proof link is shown below:

> https://monero.com/payment/e02085d31a951663f1a93c6346f89d116bc9596fd7365ae0b44cb36bc6ab7b85/86bZHZtaaCSb1mAtMbE2xF339YDhoucZu3XDLUpAFJK3X1MA4yY3j8xVKNk2ySfw5AGY2knCAyis7Be7YLZ9cKbsNUKJQT1/b4e94e0030c727c374a51f4f4b8a3f74d9503338cc3a64028c918be9f8e6ec00/

## What if I don't have the Monero transaction key?

Without the transaction key, you will need to work with the recipient for them to verify your payment. We recommend sending the following to the recipient:

* These instructions,
* The Monero transaction ID that you sent to the recipient, and
* The Monero address that you sent funds to.

The recipient should go to [Monero.com/explorer](https://monero.com/explorer). The recipient should paste the Monero transaction ID in the search box, then click the "Search" button.

[![Monero.com explorer](/images/tutorials-prove-payment-monerocom-1.png)](/images/tutorials-prove-payment-monerocom-1.png)

If the transaction record exists, it will be displayed.

The recipient should then click the "Get deposit receipt" button. The website will prompt the recipient to add their Monero address and their view key.

[![Monero.com explorer transaction details](/images/tutorials-prove-payment-monerocom-6.png)](/images/tutorials-prove-payment-monerocom-6.png)

Once added, the recipient should click the "Get deposit receipt" button. Afterwards, the website will display any outputs that were sent to that address and are associated with the provided view key.

Note: a malicious recipient can always claim that a payment was not made, even if it truly was. Please exercise coution before sending XMR to anyone, since Monero transactions are irreversible!
