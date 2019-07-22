# ADR 7: Security & Encryption

## Context and Problem Statement

*   What types of hashing and/or encryption would you leverage?
*   What data would you hash/encrypt?
*   Do you see any potential problematic areas specifically around areas like data protection, compliancy, etc.?

## Decision Drivers <!-- optional -->

*   [Crypto Shredding](https://www.thoughtworks.com/radar/techniques/crypto-shredding) – Crypto shredding is the practice of rendering sensitive data unreadable by deliberately overwriting or deleting encryption keys used to secure that data. Considering there are systems, such as audit application or blockchain, that should not or could not delete historical records, this technique is quite useful for privacy protection and GDPR compliance.
*   [General Data Protection Regulation (GDPR) Center](https://aws.amazon.com/compliance/gdpr-center/)
*   [Auto Dynamic Application Security Testing (DAST)](https://docs.gitlab.com/ee/topics/autodevops/#auto-dast-ultimate) – Dynamic Application Security Testing (DAST) uses the popular open source tool OWASP ZAProxy to perform an analysis on the current code and checks for potential security issues. The Auto DAST stage will be skipped on licenses other than Ultimate. Once the report is created, it’s uploaded as an artifact which you can later download and check out. Any security warnings are also shown in the merge request widget. Read how DAST works.

## Considered Options

*   [Valut](https://www.vaultproject.io/) – Secure, store and tightly control access to tokens, passwords, certificates, encryption keys for protecting secrets and other sensitive data using a UI, CLI, or HTTP API.
*   [Kubernetes Secrets](https://kubernetes.io/docs/concepts/configuration/secret/) – Kubernetes secret objects let you store and manage sensitive information, such as passwords, OAuth tokens, and ssh keys. Putting this information in a secret is safer and more flexible than putting it verbatim in a Pod definition or in a container image.
*   [Encrypt Data on AWS](https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingEncryption.html)
    *   Encryption of your data at rest with AES256 (EBS/S3/Glacier/RDS)
    *   Centralized managed Key Management (by AWS Region)
    *   IPsec tunnels into AWS with the VPN-Gateways
    *   Dedicated HSM modules in the cloud with AWS CloudHSM

## Decision Outcome

Chosen option: "[option 1]", because [justification. e.g., only option, which meets k.o. criterion decision driver | which resolves force force | … | comes out best (see below)].

### Positive Consequences <!-- optional -->

* [e.g., improvement of quality attribute satisfaction, follow-up decisions required, …]
* …

### Negative Consequences <!-- optional -->

* [e.g., compromising quality attribute, follow-up decisions required, …]
* …

## Pros and Cons of the Options <!-- optional -->

### [option 1]

[example | description | pointer to more information | …] <!-- optional -->

* Good, because [argument a]
* Good, because [argument b]
* Bad, because [argument c]
* … <!-- numbers of pros and cons can vary -->

### [option 2]

[example | description | pointer to more information | …] <!-- optional -->

* Good, because [argument a]
* Good, because [argument b]
* Bad, because [argument c]
* … <!-- numbers of pros and cons can vary -->

### [option 3]

[example | description | pointer to more information | …] <!-- optional -->

* Good, because [argument a]
* Good, because [argument b]
* Bad, because [argument c]
* … <!-- numbers of pros and cons can vary -->

## Links <!-- optional -->

* [Link type] [Link to ADR] <!-- example: Refined by [ADR-0005](0005-example.md) -->
* … <!-- numbers of links can vary -->
