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

### User Interface ###
![VulnerableApp-facade UI](https://raw.githubusercontent.com/SasanLabs/VulnerableApp-facade/main/docs/images/gif/VulnerableApp-Facade.gif)

## Technologies used
- Java8
- Spring Boot
- ReactJS
- Vanilla Javascript
    
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
8. [Open Redirect](https://github.com/SasanLabs/VulnerableApp/tree/master/src/main/java/org/sasanlabs/service/vulnerability/urlRedirection)
    1. [Http 3xx Status code based](https://github.com/SasanLabs/VulnerableApp/blob/master/src/main/java/org/sasanlabs/service/vulnerability/urlRedirection/Http3xxStatusCodeBasedInjection.java)

## Contributing to Project

There are multiple ways in which you can contribute to the project:
1. If you are a developer and trying to start on to the project, then the suggestion is to go through the list of [issues](https://github.com/SasanLabs/VulnerableApp/issues) which contains `good first issue` which can be a good starter.
2. If you are a developer or a security professional looking to add new Vulnerability type then you can Generate the Sample Vulnerability by running `./gradlew GenerateSampleVulnerability`. It will generate the Sample Vulnerability template which has placeholders and comments. Modified files can be seen in the logs of the command or in the github history. You can navigate to those files, fill in the placeholders and then build the project to see the effect of the changes.
3. In case you are looking to contribute to the project by publicising it or working on the growth of the project, please feel free to add your thoughts to discussions section or issues and we can discuss over them.

## Building the project
There are 2 ways in which this project can be built and used:
1. As a SringBoot application which will run with the Legacy UI or Rest API but gives the benefit of debugging and solving issues. This is the simple way, 
    1. Import the project into your favorite IDE and run it
    2. Navigate to browser and visit: `http://localhost:9090/VulnerableApp` and this will give the Legacy User Interface for VulnerableApp which you can use to debug and test.
2. As a Docker application which will help in running the full-fledged VulnerableApplication. For running as Docker application, follow following steps:
    1. Build the docker image by running `./gradlew jibDockerBuild`
    2. Download [Docker-Compose](https://github.com/SasanLabs/VulnerableApp-facade/blob/main/docker-compose.yml) and run in the same directory `docker-compose up`
    3. Navigate to browser and visit `http://localhost` and this will give the User Interface for VulnerableApp.

## Contact
In case you are stuck with any of the steps or understanding anything related to project and its goals, feel free to shoot a mail at karan.sasan@owasp.org or raise an [issue](https://github.com/SasanLabs/VulnerableApp/issues) and we will try our best to help you.

## Documentation and References

1. [Documentation](https://sasanlabs.github.io/VulnerableApp)
2. [Design Documentation](https://sasanlabs.github.io/VulnerableApp/DesignDocumentation.html)
3. [Owasp VulnerableApp](https://owasp.org/www-project-vulnerableapp/)
4. [Overview video for OWASP Spotlight series](https://www.youtube.com/watch?v=HRRTrnRgMjs)
5. [Overview Video](https://www.youtube.com/watch?v=AjL4B-WwrrA&ab_channel=OwaspVulnerableApp)

### Blogs
1. [Overview of Owasp-VulnerableApp - Medium article](https://hussaina-begum.medium.com/an-extensible-vulnerable-application-for-testing-the-vulnerability-scanning-tools-cc98f0d94dbc)
2. [Overview of Owasp-VulnerableApp - Blogspot post](https://hussaina-begum.blogspot.com/2020/10/an-extensible-vulnerable-application.html)

### Readme in other languages

1. [Russian](https://github.com/SasanLabs/VulnerableApp/tree/master/docs/i18n/ru/README.md)
2. [Chinese](https://github.com/SasanLabs/VulnerableApp/tree/master/docs/i18n/zh-CN/README.md)
3. [Hindi](https://github.com/SasanLabs/VulnerableApp/tree/master/docs/i18n/hi/README.md)
4. [Punjabi](https://github.com/SasanLabs/VulnerableApp/tree/master/docs/i18n/pa/README.md)
