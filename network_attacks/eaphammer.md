# EAPHammer

### Description
EAPHammer is a toolkit for performing targeted evil twin attacks against WPA2-Enterprise networks. It is designed to be used in full scope wireless assessments and red team engagements. As such, focus is placed on providing an easy-to-use interface that can be leveraged to execute powerful wireless attacks with minimal manual configuration. To illustrate how fast this tool is, here's an example of how to setup and execute a credential stealing evil twin attack against a WPA2-TTLS network in just two commands:

	# generate certificates
	./eaphammer --cert-wizard

	# launch attack
	./eaphammer -i wlan0 --channel 4 --auth ttls --wpa 2 --essid CorpWifi --creds

EAPHammer is also equipped to perform two new attacks [first presented at DEF CON 25](https://media.defcon.org/DEF%20CON%2025/DEF%20CON%2025%20presentations/DEFCON-25-Gabriel-Ryan-The-Black-Art-of-Wireless-Post-Exploitation-UPDATED.pdf):
 - __Hostile Portal Attacks:__ Steal Active Directory credentials without direct network access
 - __Indirect Wireless Pivots:__ Bypass port-based access controls using rogue access point attacks

Leverages a [lightly modified](https://github.com/s0lst1c3/hostapd-eaphammer) version of [hostapd-wpe](https://github.com/opensecurityresearch/hostapd-wpe) (shoutout to [Brad Anton](https://github.com/brad-anton) for creating the original), _dnsmasq_, [Responder](https://github.com/SpiderLabs/Responder), and _Python 2.7_.

### Categories
* Wireless
* Red Team
* Rogue Access Point Attacks
* WPA-EAP/WPA2-EAP

### Black Hat sessions
[![Black Hat Arsenal](https://rawgit.com/toolswatch/badges/master/arsenal/usa/2017.svg)](https://www.blackhat.com/us-17/arsenal.html#eaphammer) 
 
### Code 
https://github.com/s0lst1c3/eaphammer

### Lead Developer
 Gabriel Ryan - s0lst1c3 https://github.com/s0lst1c3

### Social Media 
* [Twitter](https://twitter.com/s0lst1c3)
* [LinkedIn](linkedin.com/in/ms08067) 
* [Blog Posts: GDS Labs](https://blog.gdssecurity.com/labs/author/gryan)
* [Blog Posts: Personal](http://solstice.me/about/)
----
