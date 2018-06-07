# Cloud Security Suite (cs-suite)
Cloud Security Suite - One stop tool for auditing the security posture of AWS infrastructure.

## Overview:
* Takes the “open source setup” pain away from you.
* Compiles all the audit checks
* Extra audit checks added
* Runs all the checks in one go
* Centralized portable reports
* Also, does local audit of the instances

## Code:
[https://github.com/SecurityFTW/cs-suite](https://github.com/SecurityFTW/cs-suite)

## Category
* Network Defense
* Infrastructure and Server Auditing

## Presented At:
[![Arsenal-2017-EU](https://rawgit.com/toolswatch/badges/master/arsenal/europe/2017.svg)](http://www.toolswatch.org/2017/09/black-hat-arsenal-europe-2017-lineup/) 

## Pre-requisites for Manual setup
* Python 2.7
* pip
* git
* gcc (for sshpass installation (OS Audit). Not a mandatory pre-requisite)
	
## Installation

```bash
git clone https://github.com/SecurityFTW/cs-suite.git
cd cs-suite/
sudo python setup.py
```

Note - Generate a set of ReadOnly AWS keys which the tool will ask to finish the installation process.

### Running cs-suite

```bash
python cs.py
```

## Documentation
[https://securityftw.github.io/Docs](https://securityftw.github.io/Docs)

## Authors
* Jayesh Singh Chauhan ([@jayeshchauhan](https://github.com/jayeshchauhan/))
* Shivankar Madaan ([@shivankar-madaan](https://github.com/shivankar-madaan))
