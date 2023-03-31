# Mimicry

<p align="center">
<img src="https://heap-web.oss-cn-hangzhou.aliyuncs.com/logo/logo_mimicry.svg" alt="Mimicry" title="Mimicry" width="120"/>
</p>

### Description


In incident response scenarios, intercepting attacks or quarantining backdoors is a common response technique. The adversarial active defense will immediately make the attacker perceive that the intrusion behavior is exposed, and the attacker may try to use defense evasion to avoid subsequent detection. This defense evasion may even result in later attacks going undetected. If we mislead or deceive the attacker into the honeypot, we can better consume the attacker's time cost and gain more response time.

We invented a series of toolkits to deceive attackers during the "kill chain." For Example:

Exploitation:
1. We return success and mislead the attacker into the honeypot for brute-force attacks.
2. We will simulate the execution of web attack payloads to deceive the existence of vulnerabilities in the system.

Post-Exploitation:
1. For the Webshell scenario, we will replace the Webshell with a proxy and transfer the Webshell to the honeypot. When the attacker accesses Webshell, the proxy will forward his request to the honeypot.
2. For the reverse shell, we will inject the shell process and forward the attacker's operation to the shell process in the honeypot.
3. For the backdoor, we will dump the process's memory, resources, etc., and migrate it to the honeypot to continue execution.

### Categories

* Network Defense
* Malware Defense
  
### Black Hat sessions

<a href="https://www.blackhat.com/eu-22/arsenal/schedule/index.html#mimicry-an-active-deception-tool-29517">
<img src="https://img.shields.io/badge/Blackhat%20Arsenal-EUROPE%202022-blue" /></a>

### Code

https://github.com/chaitin/mimicry

### Lead Developer(s)

* ChaoxinWan https://github.com/mangosteen

### Social Media
* [Twitter](https://twitter.com/unsignedjuice)
* [Discord](https://discord.gg/KjQGUrG8aJ)
