---
title: "Payment ID" 
parent: Glossary
--- 

# Payment ID

The Monero Payment ID is a [legacy feature](https://www.getmonero.org/2019/06/04/Long-Payment-ID-Deprecation.html) that is not used anymore. It was previously used as a mechanism for identitying Monero transactions as being associated with a specific account or payment.

There are several different types of Monero transaction IDs:

* Long, unencrypted payment ID. 64-hex-characters. Standalone string.
* Short, encrypted payment ID. Part of a Monero integrated address.

Long payment IDs are completely unsupported. Short payment IDs are not recommended, but they are used in rare circumstances.

The Monero community strongly recommends the use of subaddresses instead. Subaddresses provide an alternative mechanism for identifying Monero transactions as being associated with a specific account or payment.
