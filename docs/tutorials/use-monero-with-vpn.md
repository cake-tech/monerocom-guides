---
title: "Should I use Monero (XMR) with a VPN" 
parent: Tutorials
--- 

# Should I use Monero (XMR) with a VPN?

[**Monero (XMR)**](https://www.getmonero.org/) is a cryptocurrency that allows for private, untraceable payments. Using a VPN with Monero is not strictly necessary, as XMR transactions already include privacy protections by default; however, for added network privacy, you may want to use a VPN.

## What does a VPN do?

A VPN is not a catch-all that completely protects your network privacy. A VPN allows you to pick a trusted party to proxy your internet traffic through. Ultimately, you are trusting this VPN to protect your privacy. Make sure to [select a good VPN that accepts Monero (XMR) as payment](/docs/tutorials/buy-vpn-privately-monero).

A VPN has these **advantages**:

* Use of a VPN makes it harder for your internet service provider (ISP) to log your network activities.
* Use of a VPN makes it harder for websites you visit from learning your real IP address.
* VPNs are typically much simpler to use than other network privacy options.
* VPNs are typically much faster than other network privacy options.

A VPN has these **disadvantages**:

* They are centralized, and involve you needing to trust that the VPN provider — and all their infrastructure providers such as their DNS providers, server providers, etc — does not log and share your data. This can be difficult or impossible to verify.
* They do not protect your network privacy if your local device is compromised.

## What Monero (XMR) network data is potentially vulnerable?

When you send Monero (XMR) transactions, the information recorded on the blockchain (the addresses, amounts, and transaction graph) are protected by default. However, you need to communicate your transaction with the rest of the Monero network for it to be recorded in this blockchain. This necessary broadcast process leads to network privacy risk.

There are two (2) separate network connections to worry about. Your Monero wallet (for example [Cake Wallet](https://cakewallet.com)) needs to connect to a Monero node. This node then needs to other Monero nodes. Well-connected nodes may connect to hundreds at a time, but home nodes may only connect to a dozen or so.

[![Monero network diagram](/images/tutorials-use-monero-with-vpn.png){:width="100%"}](/images/tutorials-use-monero-with-vpn.png)

If you are using your [own Monero node](/docs/tutorials/monero-node) (you should!), then you need to worry about ***both*** connections. If you are using another person's node, you mostly need to worry about the first connection from your wallet device to the node.

If these connections are left unprotected, your outgoing Monero transactions could be linked to your device's IP address, or your node's IP address, depending on the case. You can also leak other metadata, such as your wallet sync progress.

## How does Monero (XMR) provide network privacy by default?

By default, Monero protects the connection between a node and other nodes on the network with Dandelion++. Dandelion++ provides basic privacy protections while transactions are being propagated across the Monero network.

With Dandelion++, nodes do not automatically share the new transactions they learn about with every node they are connected to. Instead, they will decide to follow either a "stem" or "fluff" phase. In a stem phase, a node will share the transaction with only one other node. This stem phase continues for several rounds on average, with a built-in random delay, until a node "fluffs" the transaction. This final fluff node will share the transaction with every node it is aware of. Dandelion++ transaction broadcasts thus resemble a dandelion: it's a narrow "stem" of broadcasts among only a few select nodes, before the transaction is "fluffed" at the top and distributed widely. This has the positive effect of the main transaction broadcast occuring from a different node than the node that the sender's wallet is connected to.

Dandelion++ isn't perfect. The Monero node code includes many mitigations to deal with possibly malicious nodes and other cases.

Dandelion++ isn't as comprehensive as using Tor or i2p. The Monero node software optionally supports Tor and i2p as well for users who wish to have more protection. Cake Wallet runs [an open onion node](https://guides.cakewallet.com/docs/advanced-features/custom-node/#node-lists).

**Monero does *not* provide any network protections by default between a wallet and the selected Monero node** (the first connection).

## Benefits of using a VPN with Monero (XMR)**

The most obvious reason to use a VPN with Monero is to better protect your network privacy (as a wallet user) from a Monero remote node. This is only useful if you are using someone else's node. If you are running your own node, you don't need to protect the connection between your own device and your own node.

Using a VPN will hide your real IP address from the remote node. While it can provide better metadata privacy as well, a VPN should not be relied upon for this. The only true mitigation against metadata privacy leaks is to [run your own node](/docs/tutorials/monero-node).

Using a VPN with a trusted third-party node can be good for many people's threat models. Unlike other options, a VPN is easy to set up and is very fast, which allows for reasonable Monero wallet sync progress.

## Should I use Tor or i2p instead of a VPN?

Some people prefer to use Monero with Tor or i2p, usually because they prefer to use a decentralized network instead of a single trusted party.

Tor is recommended for advanced users, but the Tor network is very slow. Syncing should not be done over Tor unless you are in a highly-sensitive environment, since performance is awful. [Read more about Monero performance over Tor in this article](https://guides.cakewallet.com/docs/advanced-features/tor-with-orbot/#performance).

Even fewer people use Monero over i2p, but some passionate users swear by this method.

## Conclusion

Should you use Monero with a VPN? It depends on your use-case, but it boils down to the following:

* Are you running your own Monero node? Then no, it's not needed!
* Are you using a third-party remote node? Then yes, you should consider using a VPN on your wallet device. Pick a [good VPN provider that accepts Monero](/docs/tutorials/buy-vpn-privately-monero).
* Are you extremely worried about your privacy? Then no, run your own node over Tor instead.
