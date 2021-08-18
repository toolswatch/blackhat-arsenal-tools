# Remote Method Guesser

### Description

*remote-method-guesser* (*rmg*) is a command line utility written in *Java* and can be used to identify security
vulnerabilities on *Java RMI* endpoints. In the following you find a list with some of it's capabilities:

* List available *bound names* and their corresponding interface class names
* List codebase locations (if exposed by the remote server)
* Check for known vulnerabilities (enabled class loader, missing *JEP290*, *JEP290* bypass, localhost bypass)
* Identify existing remote methods by using a *bruteforce* (wordlist) approach
* Call remote methods with user specified arguments (no coding required)
* Call remote methods with *ysoserial gadgets* within the arguments
* Call remote methods with a client specified codebase (remote class loading attack)
* Perform *DGC* and *registry* calls with *ysoserial* gadgets or a client specified codebase
* Perform *bind*, *unbind* and *rebind* operations against a rmi registry
* Bypass registry filtering using [An Trinhs registry bypass](https://mogwailabs.de/de/blog/2020/02/an-trinhs-rmi-registry-bypass/)
* Enumerate the unmarshalling behavior of ``java.lang.String``
* Create Java code dynamically to invoke remote methods manually

### Categories

* Vulnerability assessment
* Exploitation 
* Network attacks

### Black Hat sessions

[![BHUSA Arsenal 2021](https://raw.githubusercontent.com/toolswatch/badges/master/arsenal/usa/2021.svg)](https://www.blackhat.com/us-21/arsenal/schedule/#remote-method-guesser-a-java-rmi-vulnerability-scanner-24092)


### Code

[https://github.com/qtc-de/remote-method-guesser](https://github.com/qtc-de/remote-method-guesser)


### Lead Developer(s)

[Tobias Neitzel](https://twitter.com/qtc_de)


### Social Media

* [GitHub](https://github.com/qtc-de/remote-method-guesser)
* [Twitter](https://twitter.com/qtc_de)
* [Documentation](https://github.com/qtc-de/remote-method-guesser/tree/master/docs)
* [Slides](https://www.slideshare.net/TobiasNeitzel/remotemethodguesser-bhusa2021-arsenal)
* [Recording](https://youtu.be/t_aw1mDNhzI)
