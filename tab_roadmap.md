---
title: Roadmap
layout: null
tab: true
order: 1
tags: VulnerableApp
---

## Roadmap
### Vision for the project:

The overall vision for the project is to implement a Platform capability such that it is easier to write 
vulnerable code and exposing that through an API and UI. 

### Usage of the project:

This Project mainly targets 4 type of audience:
* Developers of Vulnerability Scanning tools
* New Vulnerability finders (for faster demonstration of the vulnerability)
* Security enthusiasts, Students who want to learn more about Security
* CTF organizers (A Platform to Host CTF by choosing vulnerabilities present in the project)

### Initial high level plan:

Basic idea for this project is to build an extensible framework which is driven by the configuration and develops who want to introduce new vulnerable code into the project need to do minimal boilerplate code and also the learning curve for configurations is minimum.

Looking at it, the first approach which comes into my mind is to give a framework similar to Spring i.e. something like annotation driven framework for including a vulnerability type and also for adding a new vulnerability to existing vulnerability type and also adding User Interface for the same. 

* Milestone 1: Alpha release - Building extensible backend Platform
* Milestone 2: Beta release - Building extensible User Interface
* Milestone 3: Gamma release - Addition of 50 vulnerabilities using the above mentioned Platform
* Milestone 4: Release 1 
* Milestone 5: Dev lifecycle integration

### Current State
For know about the current state please go to [Git Repository](https://github.com/SasanLabs/VulnerableApp) and also visit issues section for new enhancements,tech-debts and bugs.

### Timeframes
This is hard to estimate as this depends on the number of contributers but as of now i had already build some of the pieces of Backend platform and i have started building frontend platform but addition of 50 vulnerabilities can take quite a lot time. So Plan is to release this Project is near July 31 2020.

### Technology
Technologies used in this project are:

Majorly:
1. Java-8
2. SpringBoot
3. Vanila Javascript

But we are not limited to above technologies and can extend to new Horizons.
Incase you have any idea on technology and how it can suit us, please reach out to us on our [Slack-Channel](https://owasp.slack.com/messages/#owasp-vulnerableapp/).

### Challenges
There are many, please visit [Issues](https://github.com/SasanLabs/VulnerableApp/issues) for more information.
