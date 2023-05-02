---
title: "How to accept Monero (XMR) as a merchant" 
parent: Tutorials
--- 

# How to accept Monero (XMR) as a merchant

There are many tools available to accept Monero as a merchant, whether you're selling at a farmer's market or running a high-performance web store. No matter your needs, this guide will help you pick the best method to simply receive Monero (XMR) payments!

## A note on fiat conversions

Depending on your needs, you may wish to retain the received Monero, or you may wish to convert to your local fiat currency. This latter method may be ideal if you need to pay your suppliers in fiat, for example. This guide includes your best options for converting to fiat in each of the methods.

## For manual invoices: Cake Wallet receive screen

[Cake Wallet](https://cakewallet.com) makes it extremely simple to accept payments in Monero, if you are a merchant who only expects to receive a few payments in Monero. Accepting Monero payments is as simple as downloading the free app and sending your wallet address or invoice link to people.

1. **Create a Monero Wallet:** The first step is to create a Monero wallet to store the Monero coins you receive as payment. You can use a [software wallet](/docs/app-support/app-support) like [Cake Wallet](https://cakewallet.com) to get started instantly. It's important to have a secure backup of the seed in case anything goes wrong.

2. **Get a payment address or invoice link:** To receive Monero payments, you need to share your Monero payment address with your customers. You can display this on your website or in-person using a QR code or a payment button. Use the receive screen QR code if you only need to track 1 invoice at a time. Use the invoice feature if you need to track multiple at a time.

	a. **If you are tracking one payment at a time:** Simply use the receive screen address. Copy it, and give the address to the customer.

	[![Cake Wallet receive screen](/images/tutorials-accept-monero-as-merchant-1.jpg){:width="32%"}](/images/tutorials-accept-monero-as-merchant-1.jpg)

	b. **If you are tracking several payments at a time:** Follow [these simple instructions](https://guides.cakewallet.com/docs/advanced-features/trocador-anonpay/#create-invoices) to use the Trocador AnonPay Invoice feature. This includes advanced options, such as invoice tracking.

	[![Cake Wallet invoice screen](/images/tutorials-accept-monero-as-merchant-2.jpg){:width="32%"}](/images/tutorials-accept-monero-as-merchant-2.jpg)
    
3. **Ask the customer for payment:** Give the customer the Monero address or invoice payment link. Tell them to send a specific amount of XMR or an equivalent amount in fiat (eg: USD) to you. 
    
4. **Verify payment:** You can confirm payment in the Monero transactions history screen. Open Cake Wallet and swipe right to left from the home screen. If a payment was made to that wallet, you should see an incoming transaction with the fiat or crypto value that you specified to the customer. If there is a dispute, work with the customer. Incoming Monero transactions need 10 cofirmations (about 20 minutes) before they can be transferred again.

### Converting to fiat

Your simplest options to convert this Monero (XMR) to fiat are:

* Send Monero to an exchange that supports Monero (eg: Binance and Kraken), and then convert to fiat.
* Convert Monero to Bitcoin [in Cake Wallet](https://guides.cakewallet.com/docs/basic-features/exchange/), then sell Bitcoin to fiat in Cake Wallet.
* Sell Monero on LocalMonero.

## For simple web stores: NOWPayments

[NOWPayments](https://nowpayments.io/) makes it easy to accept Monero at your web store. Fees start at 0.5% (plus exchange spreads). You can austomatically convert the received funds to the cryptocurrency of your choice such as a stablecoin (USDT, USDC, DAI), or the fiat currency EUR (requires additional verification).

There are plugins for popular ecommerce platforms [Shopify](https://nowpayments.io/payment-integration/shopify-plugin), [WooCommerce](https://nowpayments.io/woocommerce-plugin), [OpenCart](https://nowpayments.io/opencart-plugin), [ECWID](https://nowpayments.io/payment-integration/ecwid-plugin), [WHMCS](https://nowpayments.io/whmcs-plugin), [PrestaShop](https://nowpayments.io/payment-integration/prestashop-plugin), [Magneto2](https://nowpayments.io/magento-2-plugin), [Zen Cart](https://nowpayments.io/payment-integration/zen-cart-plugin), [Shopware](https://nowpayments.io/payment-integration/shopware-plugin), or you can use [their API](https://documenter.getpostman.com/view/7907941/2s93JusNJt) for a custom integration.

### Converting to fiat

You can use their integration with [Switchere](https://switchere.com/) to receive EUR payments with SEPA, but we do not recommend this route since fees are 1.5% to 2.3% extra.

We recommend settling in a stablecoin such as USDT, USDC, or DAI, and then sending that stablecoin to an exchange periodically. Good exchange options include Kraken, Binance, and Coinbase. Going through [Coinbase](https://help.coinbase.com/en/business-onboarding) or [Circle](https://www.circle.com/en/circle-account) makes the most sense if you have high volumes, since you can convert stablecoins to fiat for almost free.

## For complex web stores: BTCPay Server

Despite its name, [BTCPay Server](https://btcpayserver.org/) is a robust option for accepting payments in Monero in addition to Bitcoin and a few other assets. This option is perfect for any custom implementation. It's open-source.

[Follow Seth for Privacy's guide](https://sethforprivacy.com/guides/accepting-monero-via-btcpay-server/) to set up a server and configure it for accepting Monero payments.

### Converting to fiat

You will need to run a task to auto-transfer and then auto-convert the Monero to fiat. We have written several Python scripts that handle these tasks on Kraken, which you can view [here](https://github.com/cake-tech/autoforward-autoconvert).

## Alternative: Anypay

[Anypay](https://anypayx.com/) supports custom implementations for accepting Monero payments.

## Alternative: Monero Integrations

[Monero Integrations](https://monerointegrations.com/) is a set of open-source plugins for many Content Management Systems (CMS).
