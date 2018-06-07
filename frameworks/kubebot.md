# Kubebot

### Description
Kubebot is an automated scalable security testing framework based on a microservice architecture. Requests are sent to an API server which then orchestrates running the tools as Docker containers on a Kubernetes (K8S) backend. These requests are asynchronous i.e. they get dropped in a queue which are then picked up by Subscription workers. The subscription workers start the job of running the tools. The results of running those tools are diff'ed and only the changes are sent back to the fronend.

Kubebot uses Slack as the frontend - as a way to send API requests but this can be extended into different frontends as well.

Kubebot also gives the flexibility of setting up scheduled job runs using the K8S cronjob.


### Categories
* Frameworks
* Security Testing
* BugBounty
* Automation
* Containers


### Black Hat sessions
[![Arsenal](https://rawgit.com/toolswatch/badges/master/arsenal/usa/2017.svg)](http://www.toolswatch.org/2017/06/the-black-hat-arsenal-usa-2017-phenomenal-line-up-announced/)


### Code
https://github.com/anshumanbh/kubebot


### Lead Developer
 Anshuman Bhartiya - anshumanbh https://github.com/anshumanbh

### Social Media
* [Twitter](https://twitter.com/anshuman_bh)
* [DevSecOps](https://github.com/devsecops)
