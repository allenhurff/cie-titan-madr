# ADR 6: Authorization and Authentication

## Context and Problem Statement

*   How will you handle authorization and authentication?
*   How will you differentiate between the various types of roles?
*   How would you manage access and security on the API level to restrict access to other team data?

## Decision Drivers <!-- optional -->

* [driver 1, e.g., a force, facing concern, …]
* [driver 2, e.g., a force, facing concern, …]
* … <!-- numbers of drivers can vary -->

## Considered Options

*   [AWS Organizations](https://aws.amazon.com/organizations/) – AWS Organizations helps you centrally govern your environment as you grow and scale your workloads on AWS. Whether you are a growing startup or a large enterprise, Organizations helps you to centrally manage billing; control access, compliance, and security; and share resources across your AWS accounts. Using AWS Organizations, you can automate account creation, create groups of accounts to reflect your business needs, and apply policies for these groups for governance. You can also simplify billing by setting up a single payment method for all of your AWS accounts. Through integrations with other AWS services, you can use Organizations to define central configurations and resource sharing across accounts in your organization. AWS Organizations is available to all AWS customers at no additional charge.
*   [Amazon Cognito](https://aws.amazon.com/cognito/) – Amazon Cognito lets you add user sign-up, sign-in, and access control to your web and mobile apps quickly and easily. Amazon Cognito scales to millions of users and supports sign-in with social identity providers, such as Facebook, Google, and Amazon, and enterprise identity providers via SAML 2.0.
*   [Auth0 B2E](https://auth0.com/b2e-identity-management-for-employees/) – Auth0 provides authentication and authorization as a service. Token-based Single Sign On for your Apps and APIs with social, databases and enterprise identities.

## Decision Outcome

Chosen option: "[option 1]", because [justification. e.g., only option, which meets k.o. criterion decision driver | which resolves force force | … | comes out best (see below)].
