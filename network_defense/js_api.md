# Protecting your Crypto Asset against Malicious JS Phishing

### Description
Cryptocurrencies and NFT are taking over with predictions of 90% of the population holding at least one of them by the end of the decade. Users that want to facilitate these new assets, trade them and sell them typically do that using wallets, and in particular hot wallets that are easy-to-use. The most popular hot wallets today (e.g., MetaMask) are browser based and are thus vulnerable to phishing and scams made possible through malicious JavaScript, such as a recent campaign carried out by the Lazarus group which resulted in more than 400M$ worth of stolen cryptocurrencies.

We release our internal tool used by the Security Operation and the research at Akamai to scan the JS from any website.
It includes a Python recursive crawler that extracts every JS from any domain (written within the HTML or imported), analyzes it with a model and heuristics - that we provide -, and brings metadata ( from VT, publicwww…) It finally gives a score to every piece of code running on any URL of a specified domain.
The code works also as a Web App and exposes a REST API as well.

We will finish by presenting some real detection we caught with this tool and explaining them.
### Categories

* Network Defense

### Black Hat sessions

[![Arsenal](https://raw.githubusercontent.com/toolswatch/badges/d50ddaf5b003dc503a2c9a33a85d2a1e3d57b40c/arsenal/usa/2022.svg)](https://www.blackhat.com/us-22/arsenal/schedule/#protecting-your-crypto-asset-against-malicious-js-phishing-27713)


### Popularity

To be completed

### Code
https://github.com/akamai/js_api

### Lead Developer(s)

**Code**: [Jordan Garzon]
**Aknoledgment**:[Asaf Nadler]

from [Akamai Technologies](https://www.akamai.com)


[Jordan Garzon]: https://twitter.com/JordGarzon
[Asaf Nadler]: https://twitter.com/AsafNadler