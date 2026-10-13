Version: NAFATH-V4
Track: Cybersecurity

## Overview

A national service provider depends on secure software, artificial intelligence, mobile applications, networks, cybersecurity, and reliable data to deliver trusted services. Each area introduces risks that must be identified and managed. Secure software configuration keeps secrets out of source code and reduces the risk of exposure. AI security addresses attacks that manipulate model inputs or training data. Mobile security verification helps teams assess application weaknesses before release. Network security protects internet traffic from route manipulation and interception. Cybersecurity practices help organisations identify and fix serious software vulnerabilities. Software component transparency helps teams understand dependencies and respond to newly discovered threats. These six areas are connected because a weakness in one component can affect the security and reliability of the entire service. Protecting national services therefore requires verification, monitoring, and coordinated security controls. This mission also examines how software configuration and secret management reduce security risks.


## Software

The Twelve-Factor App methodology recommends storing configuration in environment variables instead of hard-coding it in source code. Configuration may include database credentials and external service keys. Keeping these values outside the code reduces the risk of exposing secrets when code is shared or published. It also allows settings to change between development and production without modifying the application. Secrets must still be protected through appropriate access controls and secure deployment practices.

Resource: The Twelve-Factor App - Config - https://12factor.net/config

## AI

Artificial intelligence systems can be vulnerable to adversarial machine learning attacks. These attacks may manipulate input data or training data to affect a model’s behaviour and results. The National Institute of Standards and Technology (NIST) explains different types of attacks and approaches for mitigating their effects. Organisations should assess AI systems throughout their life cycle, protect training data, test models against potential attacks, and monitor their performance. These measures help reduce security risks and improve the reliability of AI systems used in essential services.

Resource: NIST - Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations - https://www.nist.gov/publications/adversarial-machine-learning-taxonomy-and-terminology-attacks-and-mitigations-0


## Mobile

Mobile applications can contain security weaknesses that expose sensitive information or allow attackers to misuse application features. The OWASP Mobile Application Security Testing Guide (MASTG) provides guidance for testing mobile applications and identifying vulnerabilities. Security testing should examine data storage, authentication, network communication, and the way applications handle sensitive information. Developers should test applications throughout development, fix identified weaknesses, and verify that security controls work as expected. These practices help reduce risks and protect users and their data.

Resource: OWASP - Mobile Application Security Testing Guide (MASTG) - https://mas.owasp.org/MASTG/


## Networking

Network security helps protect data as it travels between systems. The OWASP Transport Layer Protection Cheat Sheet recommends using Transport Layer Security (TLS) correctly to protect communications against eavesdropping and tampering. Organisations should use modern, secure TLS configurations, validate digital certificates, and avoid outdated protocols and weak cipher suites. They should also ensure that sensitive information is transmitted over encrypted connections. These measures help protect user data, maintain communication integrity, and reduce the risk of network-based attacks.

Resource: OWASP - Transport Layer Protection Cheat Sheet - https://cheatsheetseries.owasp.org/cheatsheets/Transport_Layer_Protection_Cheat_Sheet.html


## Cybersecurity

Secure coding practices help reduce vulnerabilities throughout the software development process. OWASP’s Secure Coding Practices Quick Reference Guide covers important areas such as input validation, authentication, access control, error handling, and data protection. Developers should validate input from untrusted sources, restrict access to authorised users, avoid exposing sensitive information in error messages, and protect data during storage and transmission. Regular code reviews and security testing can help identify weaknesses before applications are deployed. Applying these practices improves software security and helps protect essential digital services.

Resource: OWASP - Secure Coding Practices Quick Reference Guide - https://owasp.org/www-project-secure-coding-practices-quick-reference-guide/

## Data

Software transparency helps organisations understand the components and dependencies used in their applications. The National Telecommunications and Information Administration (NTIA) explains that a Software Bill of Materials (SBOM) records information about software components and their relationships. This information helps organisations identify affected components when new vulnerabilities are discovered and respond more quickly to security risks. An SBOM should include details such as component names, versions, suppliers, and dependency relationships. Keeping this information accurate and up to date supports vulnerability management and improves software supply chain security. However, an SBOM does not eliminate vulnerabilities on its own; organisations must use it alongside security testing and regular monitoring.

Resource: NTIA - The Minimum Elements for a Software Bill of Materials (SBOM) - https://www.ntia.gov/report/2021/minimum-elements-software-bill-materials-sbom

## Misconception in My Track

A common misconception in cybersecurity is that using antivirus software or a firewall is enough to keep an organisation completely secure. Although these tools are important, they cannot prevent every attack or eliminate all vulnerabilities. The Cybersecurity and Infrastructure Security Agency (CISA) recommends a layered approach to cybersecurity that combines technical controls, secure configurations, regular updates, access management, and user awareness. Organisations should also monitor systems, test security measures, and prepare to respond to incidents. Effective cybersecurity requires continuous risk management rather than relying on a single security tool.

Resource: CISA - Cybersecurity Best Practices - https://www.cisa.gov/topics/cybersecurity-best-practices

## Open Question

How can national service providers balance the use of emerging technologies, such as artificial intelligence and mobile applications, with the need to protect sensitive data and maintain reliable services? What combination of security testing, software transparency, secure configuration, and continuous monitoring would be most effective in reducing risks across the entire service?

Resource: NIST - Cybersecurity Framework (CSF) 2.0 - https://www.nist.gov/cyberframework







