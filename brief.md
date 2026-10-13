Version: NAFATH-V4
Track: Cybersecurity

## Overview

A national service provider depends on secure software, artificial intelligence, mobile applications, networks, cybersecurity, and reliable data to deliver trusted services. Each area introduces risks that must be identified and managed. Secure software configuration keeps secrets out of source code and reduces the risk of exposure. AI security addresses attacks that manipulate model inputs or training data. Mobile security verification helps teams assess application weaknesses before release.

Network security protects internet traffic from route manipulation and interception. Cybersecurity practices help organisations identify and fix serious software vulnerabilities. Software component transparency helps teams understand dependencies and respond to newly discovered threats. These six areas are connected because a weakness in one component can affect the security and reliability of the entire service.

Protecting national services therefore requires verification, monitoring, and coordinated security controls. This mission also examines the Log4Shell vulnerability and its mitigation.


## Software

The Twelve-Factor App methodology recommends storing configuration in environment variables rather than hard-coding it in source code. Configuration may include database credentials and external service keys. Keeping these values outside the code reduces the risk of exposing them when code is shared or published. However, environment variables alone do not guarantee security; access controls and secure deployment practices are also necessary to protect sensitive values.

Resource: The Twelve-Factor App - Config - https://12factor.net/config

## AI

Adversarial machine learning attacks can target different stages of an AI system. Evasion attacks manipulate inputs at inference time to make a trained model produce incorrect predictions. In contrast, poisoning attacks manipulate training data or the training process to influence the model’s behaviour. The key difference is that evasion targets how a model responds to inputs, while poisoning affects how it learns. Organisations should test models against adversarial inputs, protect training-data integrity, and monitor model performance.

Resource: NIST - Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations - https://www.nist.gov/publications/adversarial-machine-learning-taxonomy-and-terminology-attacks-and-mitigations-0

## Mobile

The OWASP Mobile Application Security Verification Standard (MASVS) defines security requirements for mobile applications. It helps developers and testers assess security controls in areas such as secure storage, cryptography, authentication, network communication, and platform interaction. Teams can use MASVS to guide security testing, identify weaknesses, and determine whether an application meets relevant security requirements. Applying the standard during development helps protect sensitive information and improve mobile application security.

Resource: OWASP - Mobile Application Security Verification Standard (MASVS) - https://mas.owasp.org/MASVS/

## Networking

BGP route hijacking occurs when an autonomous system announces incorrect or unauthorised internet routes, potentially diverting traffic through an unintended network. Resource Public Key Infrastructure (RPKI) helps reduce this risk by allowing networks to validate whether a route announcement is authorised by the holder of the relevant IP address resources. However, RPKI does not encrypt traffic or prevent every routing attack. Its protection depends on networks performing route-origin validation. Organisations should combine RPKI validation with other routing security practices.

Resource: RIPE NCC - Resource Public Key Infrastructure (RPKI) - https://www.ripe.net/manage-ips-and-asns/resource-management/rpki/

## Cybersecurity

Log4Shell (CVE-2021-44228) was a critical vulnerability in Apache Log4j, a widely used Java logging library. It could allow attackers to execute malicious code remotely on vulnerable systems by sending specially crafted input that Log4j processed. Its severity came from the library’s widespread use and the potential for serious compromise without direct access to the target system. Organisations should update affected Log4j versions to fixed releases, identify vulnerable applications and dependencies, and follow vendor security guidance.

Resource: CISA - Apache Log4j Vulnerability Guidance - https://www.cisa.gov/news-events/cybersecurity-advisories/aa21-356a

## Data

A Software Bill of Materials (SBOM) is a structured inventory of software components and their relationships. It helps organisations identify affected dependencies when vulnerabilities are discovered and improve software supply chain security. The NTIA identifies minimum SBOM elements including supplier name, component name, component version, other unique identifiers, dependency relationships, SBOM author, and timestamp. Keeping an SBOM accurate and up to date helps teams understand what software they use and respond to security risks. However, an SBOM does not remove vulnerabilities; it supports security analysis and remediation.

Resource: NTIA - The Minimum Elements for a Software Bill of Materials (SBOM) - https://www.ntia.gov/report/2021/minimum-elements-software-bill-materials-sbom

## Misconception in My Track

A common misconception is that installing a security update once means an organisation is fully protected from a vulnerability such as Log4Shell. In reality, teams must first identify all affected applications and software dependencies, including systems that may bundle vulnerable versions of Log4j. They must then apply fixed versions, verify that the updates succeeded, and check for any signs of exploitation. Patching one visible server may not fix every affected component. CISA’s guidance, under the section discussing mitigation and remediation, explains the need to identify affected products and take corrective action. Security therefore requires verification, not just installing an update.

Resource: CISA - Apache Log4j Vulnerability Guidance - https://www.cisa.gov/news-events/cybersecurity-advisories/aa21-356a

## Open Question

How can an organisation reliably identify every application and software dependency affected by a newly discovered vulnerability such as Log4Shell, especially when third-party components are not fully documented?






