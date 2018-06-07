

# WSSAT - Web Service Security Assessment Tool

### Description
WSSAT is an open source web service security scanning tool which provides a dynamic environment to add, update or delete vulnerabilities by just editing its configuration files. This tool accepts WSDL address list as input file and for each service, it performs both static and dynamic tests against the security vulnerabilities. It also makes information disclosure controls.
With this tool, all web services could be analysed at once and the overall security assessment could be seen by the organization.

**Objectives of WSSAT are to allow organizations:**
* Perform their web services security analysis at once
* See overall security assessment with reports
* Harden their web services

# WSSAT 2.0
**REST API** scanning support was added with same dynamic vulnerability management environment philosophy as SOAP services. [ChangeLog](https://github.com/YalcinYolalan/WSSAT/blob/master/CHANGELOG.md)

**WSSAT’s main capabilities include:**

**Dynamic Testing:**
* Insecure Communication - SSL Not Used
* Unauthenticated Service Method
* Error Based SQL Injection
* Cross Site Scripting
* XML Bomb
* External Entity Attack - XXE
* XPATH Injection
* Verbose SOAP Fault Message

**Static Analysis:**
* Weak XML Schema: Unbounded Occurrences
* Weak XML Schema: Undefined Namespace
* Weak WS-SecurityPolicy: Insecure Transport
* Weak WS-SecurityPolicy: Insufficient Supporting Token Protection
* Weak WS-SecurityPolicy: Tokens Not Protected

**Information Leakage:**
* Server or technology information disclosure

**WSSAT’s main modules are:**
* Parser
* Vulnerabilities Loader
* Analyzer/Attacker
* Logger
* Report Generator

The main difference of WSSAT is to create a dynamic vulnerability management environment instead of embedding the vulnerabilities into the code.

_This project has been started as Term Project at Middle East Technical University (METU), Software Management master program._

### Categories

* Web Application
* Web Service
* Pentest
* Vulnerability assessment

### Black Hat sessions

[![Black Hat Arsenal USA](https://rawgit.com/toolswatch/badges/master/arsenal/usa/2016.svg)](https://www.blackhat.com/us-16/arsenal.html#web-service-security-assessment-tool-wssat) 
[![Black Hat Arsenal Europe](https://rawgit.com/toolswatch/badges/master/arsenal/europe/2016.svg)](https://www.blackhat.com/eu-16/arsenal.html#wssat-web-service-security-assessment-tool)

### Code
https://github.com/YalcinYolalan/WSSAT

### Lead Developers

- Mehmet Yalçın YOLALAN (https://www.linkedin.com/in/yalcinyolalan/)
- Salih TALAY (https://www.linkedin.com/in/salih-talay-49025238/)

### Social Media

* [Project homepage](http://yalcinyolalan.github.io/WSSAT/)


