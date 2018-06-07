# gr-lora

### Description
gr-lora is an open-source GNU Radio/Software Defined Radio implementation of the LoRa radio physical layer, as derived from the author's black box analysis of the protocol. gr-lora empowers developers and security researchers to think beyond packet sniffing and injection by exposing LoRa's physical layer in software.

LoRa is a wireless networking technology that can be thought of as high-endurance cellular for IoT and embedded devices. It utilizes a unique Chirp Spread Spectrum modulation and layered encoding scheme to achieve remarkable range while remaining frugal on power.

PHYs have long been taken for granted, however research such as Travis Goodspeed's packet-in-packet and Dartmouth/River Loop Security's 802.15.4 chipset fingerprinting have demonstrated that physical layer abuse can have severe consequences further up the stack. As a closed protocol, LoRa has only been exposed via layer 2+ interfaces; thus security researchers and developers have lacked the necessary tools to audit and analyze the security and robustness of its PHY.

With its flexible and open architecture, gr-lora gives security researchers the capability required to explore this nascent protocol from its most fundamental layer.

For more information on the LoRa PHY and Matt's blind signal analysis process:
* 33c3 Video: https://media.ccc.de/v/33c3-7945-decoding_the_lora_phy
* PoC||GTFO 0x13: https://www.alchemistowl.org/pocorgtfo/pocorgtfo13.pdf

### Categories
* Network Attacks
* Wireless
* Reverse Engineering
* Hardware/IoT

### Black Hat sessions
[![Arsenal](https://rawgit.com/toolswatch/badges/master/arsenal/usa/2017.svg)](https://www.blackhat.com/us-17/arsenal/schedule/index.html#gr-lora-an-open-source-sdr-implementation-of-the-lora-phy-8045)
 
### Code 
https://github.com/BastilleResearch/gr-lora

### Lead Developer
 Matt Knight - https://github.com/matt-knight

### Social Media 
* [Twitter](https://twitter.com/embeddedsec)
* [Company Website](https://bastille.net) 

----

