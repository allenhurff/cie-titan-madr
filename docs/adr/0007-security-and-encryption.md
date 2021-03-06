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
*   [AWS Secrets Manager](https://aws.amazon.com/secrets-manager/) helps you protect secrets needed to access your applications, services, and IT resources. The service enables you to easily rotate, manage, and retrieve database credentials, API keys, and other secrets throughout their lifecycle. Users and applications retrieve secrets with a call to Secrets Manager APIs, eliminating the need to hardcode sensitive information in plain text. Secrets Manager offers secret rotation with built-in integration for Amazon RDS, Amazon Redshift, and Amazon DocumentDB. Also, the service is extensible to other types of secrets, including API keys and OAuth tokens. In addition, Secrets Manager enables you to control access to secrets using fine-grained permissions and audit secret rotation centrally for resources in the AWS Cloud, third-party services, and on-premises.

## Decision Outcome

*    Kubernetes Secrets
*    AWS Secrets Manager
