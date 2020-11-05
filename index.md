---

layout: col-sidebar
title: OWASP VulnerableApp
tags: VulnerableApp
level: 2
type: code
pitch: VulnerableApp is a delibrately Vulnerable Web Application for Vulnerability Scanning Tool developers, its consumers and students. 

---
![VulnerableApp Logo](https://raw.githubusercontent.com/SasanLabs/VulnerableApp/master/docs/logos/Coloured/iconColoured.png) 


![OWASP Incubator](https://img.shields.io/badge/owasp-incubator-blue.svg) [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) ![Java CI with Gradle](https://github.com/SasanLabs/VulnerableApp/workflows/Java%20CI%20with%20Gradle/badge.svg) [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

As Web Applications are becoming popular these days, there comes a dire need to secure them. Although there are several Vulnerability Scanning Tools, however while developing these tools, developers need to test them. Moreover, they also need to know how well is the Vulnerability Scanning tool performing. As of now, there are little or no such vulnerable applications existing for testing such tools. There are Deliberately Vulnerable Applications existing in the market but they are not written with such an intent and hence lag extensibility, e.g. adding new vulnerabilities is quite difficult. Hence, the developers resort to writing their own vulnerable applications, which usually causes productivity loss and the pain to rework.

**VulnerableApp** is built keeping these factors in mind. This project is scalable, extensible, easier to integrate and easier to learn.
As solving the above issue requires addition of various vulnerabilities, hence it becomes a very good platform to learn various security vulnerabilities.

## Currently handled Vulnerability types

1. [JWT Vulnerability](https://github.com/SasanLabs/VulnerableApp/blob/master/src/main/java/org/sasanlabs/service/vulnerability/jwt/)
2. [Command Injection](https://github.com/SasanLabs/VulnerableApp/tree/master/src/main/java/org/sasanlabs/service/vulnerability/commandInjection)
3. [File Upload Vulnerability](https://github.com/SasanLabs/VulnerableApp/tree/master/src/main/java/org/sasanlabs/service/vulnerability/fileupload)
4. [Path Traversal Vulnerability](https://github.com/SasanLabs/VulnerableApp/tree/master/src/main/java/org/sasanlabs/service/vulnerability/pathTraversal)
5. [SQL Injection](https://github.com/SasanLabs/VulnerableApp/tree/master/src/main/java/org/sasanlabs/service/vulnerability/sqlInjection)
    1. [Error Based SQLi](https://github.com/SasanLabs/VulnerableApp/blob/master/src/main/java/org/sasanlabs/service/vulnerability/sqlInjection/ErrorBasedSQLInjectionVulnerability.java)
    2. [Union Based SQLi](https://github.com/SasanLabs/VulnerableApp/blob/master/src/main/java/org/sasanlabs/service/vulnerability/sqlInjection/UnionBasedSQLInjectionVulnerability.java)
    3. [Blind SQLi](https://github.com/SasanLabs/VulnerableApp/blob/master/src/main/java/org/sasanlabs/service/vulnerability/sqlInjection/BlindSQLInjectionVulnerability.java)
6. [XSS](https://github.com/SasanLabs/VulnerableApp/tree/master/src/main/java/org/sasanlabs/service/vulnerability/xss)
    1. [Persistent XSS](https://github.com/SasanLabs/VulnerableApp/tree/master/src/main/java/org/sasanlabs/service/vulnerability/xss/persistent)
    2. [Reflected XSS](https://github.com/SasanLabs/VulnerableApp/tree/master/src/main/java/org/sasanlabs/service/vulnerability/xss/reflected)
7. [XXE](https://github.com/SasanLabs/VulnerableApp/tree/master/src/main/java/org/sasanlabs/service/vulnerability/xxe)

### Future Goal
Going further, this application might becomes a database for vulnerabilities. Hence, in future, it can be used for hosting CTFs and can also become a compliance/benchmark for Vulnerability Scanning tools.

# Contribution
Everyone is welcome and encouraged to participate in our [Project](https://github.com/SasanLabs/VulnerableApp).

# Communication
Please feel free to reach out to us on our [VulnerableApp Slack Channel](https://owasp.slack.com/messages/#owasp-vulnerableapp/) or send an email to karan.sasan@owasp.org for any queries.

OWASP is a fantastic place to learn about application security, to network, and even
to build your reputation as an expert. We also encourage you to be [become a member](/membership) or consider
a [donation](/donate?reponame=www-project-vulnerableapp&title=OWASP+VulnerableApp) to support our ongoing work.

[More Information on Project](https://sasanlabs.github.io/VulnerableApp/)

## Blogs/Documentations and other details
1. [Documentation](https://sasanlabs.github.io/VulnerableApp)
2. [Overview Video](https://www.youtube.com/watch?v=AjL4B-WwrrA&ab_channel=OwaspVulnerableApp)
3. [Overview of Owasp-VulnerableApp - Medium article](https://hussaina-begum.medium.com/an-extensible-vulnerable-application-for-testing-the-vulnerability-scanning-tools-cc98f0d94dbc)
4. [Overview of Owasp-VulnerableApp - Blogspot post](https://hussaina-begum.blogspot.com/2020/10/an-extensible-vulnerable-application.html)

