# OSfooler

### Description
An outsider has the capability to discover general information, such as which operating system a host is running, by searching for default stack parameters, ambiguities in IETF RFCs or non-compliant TCP/IP implementations in responses to malformed requests. By pinpointing the exact OS of a host, an attacker can launch an educated and precise attack against a target machine.

There are lot of reasons to hide your OS to the entire world:
 * Revealing your OS makes things easier to find and successfully run an exploit against any of your devices.
 * Having and unpatched or antique OS version is not very convenient for your company prestige. Imagine that your company is a bank and some users notice that you are running an unpatched box. They won't trust you any longer! In addition, these kind of 'bad' news are always sent to the public opinion.
 * Knowing your OS can also become more dangerous, because people can guess which applications are you running in that OS (data inference). For example if your system is a MS Windows, and you are running a database, it's highly likely that you are running MS-SQL.
 * It could be convenient for other software companies, to offer you a new OS environment (because they know which you are running).
 * And finally, privacy; nobody needs to know the systems you've got running.

OSfooler was presented at Blackhat Arsenal 2013. It was built on NFQUEUE, an iptables/ip6tables target which delegate the decision on packets to a userspace. It transparently intercepted all traffic that your box was sending in order to camouflage and modify in real time the flags in TCP/IP packets that discover your system. Detects and defeat at the same time:
 * Active remote OS fingerprinting: like Nmap
 * Passive remote OS fingeprinting: like p0f v2
 * Commercial engines like Sourcefire’s FireSiGHT OS fingerprinting

Some additional features are:
 * No need for kernel modification or patches
 * Simple user interface and several logging features
 * Transparent for users, internal process and services
 * Detecting and defeating mode: active, passive & combined
 * Will emulate any OS
 * Capable of handling updated nmap and p0f v2 fingerprint database
 * Undetectable for the attacker

### Categories
* Network Defense
* Hardening

### Black Hat sessions
[![Arsenal](https://github.com/toolswatch/badges/blob/master/arsenal/usa/2013.svg)](https://www.toolswatch.org/2013/06/announcement-blackhat-arsenal-usa-2013-selected-tools/)

### Code
https://github.com/segofensiva/OSfooler-ng

### Lead Developer(s)
Jaime Sánchez - aka @segofensiva -

### Social Media
* [Twitter](https://twitter.com/segofensiva)
* [Blog](https://seguridadofensiva.com/)