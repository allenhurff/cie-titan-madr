# ADR 13: Deployments

## Context and Problem Statement

*   What Is your plan for managing builds and deployments across the various environments? Which and how many environments would you plan to support?

## Decision Drivers <!-- optional -->

*   [Getting Started with Helm/Tiller in Kubernetes](https://medium.com/@anthonyganga/getting-started-with-helm-tiller-in-kubernetes-part-one-3250aa99c6ac)

## Considered Options

*   [GitLab's AutoDevOps](https://docs.gitlab.com/ee/topics/autodevops/) – Auto DevOps provides pre-defined CI/CD configuration which allows you to automatically detect, build, test, deploy, and monitor your applications. Leveraging CI/CD best practices and tools, Auto DevOps aims to simplify the setup and execution of a mature & modern software development lifecycle.
*   [Jenkin's X](https://jenkins-x.io/) – Jenkins X provides pipeline automation, built-in GitOps and preview environments to help teams collaborate and accelerate their software delivery at any scale.
*   [AWS CodeDeploy](https://aws.amazon.com/codedeploy/) – AWS CodeDeploy is a fully managed deployment service that automates software deployments to a variety of compute services such as Amazon EC2, AWS Fargate, AWS Lambda, and your on-premises servers. AWS CodeDeploy makes it easier for you to rapidly release new features, helps you avoid downtime during application deployment, and handles the complexity of updating your applications. You can use AWS CodeDeploy to automate software deployments, eliminating the need for error-prone manual operations. The service scales to match your deployment needs.
*   [CircleCI](https://circleci.com/) – Continuous integration and delivery platform helps software teams rapidly release code with confidence by automating the build, test, and deploy process. Offers a modern software development platform that lets teams ramp
*   [GitLab Runner (cirunner)](https://docs.gitlab.com/runner/) – GitLab Runner is the open source project that is used to run your jobs and send the results back to GitLab. It is used in conjunction with GitLab CI, the open-source continuous integration service included with GitLab that coordinates the jobs.
*   [Kubernetes](kubernetes.io) – is an open-source system for automating deployment, scaling, and management of containerized applications.
*   [Helm/Tiller](https://helm.sh/) – helps you manage Kubernetes applications — Helm Charts help you define, install, and upgrade even the most complex Kubernetes application. Charts are easy to create, version, share, and publish — so start using Helm and stop the copy-and-paste.
*   [Kops](https://github.com/kubernetes/kops) – helps you create, destroy, upgrade and maintain production-grade, highly available, Kubernetes clusters from the command line. AWS (Amazon Web Services) is currently officially supported, with GCE in beta support , and VMware vSphere in alpha, and other platforms planned.
*   [Terraform](https://www.terraform.io/) – enables you to safely and predictably create, change, and improve infrastructure. It is an open source tool that codifies APIs into declarative configuration files that can be shared amongst team members, treated as code, edited, reviewed, and versioned.
*   [AWS EKS](https://aws.amazon.com/eks/) – runs the Kubernetes management infrastructure for you across multiple AWS availability zones to eliminate a single point of failure. Amazon EKS is certified Kubernetes conformant so you can use existing tooling and plugins from partners and the Kubernetes community. Applications running on any standard Kubernetes environment are fully compatible and can be easily migrated to Amazon EKS.
*   [AWS ECR](https://aws.amazon.com/ecr/) – is a fully-managed Docker container registry that makes it easy for developers to store, manage, and deploy Docker container images. Amazon ECR is integrated with Amazon Elastic Container Service (ECS), simplifying your development to production workflow. Amazon ECR eliminates the need to operate your own container repositories or worry about scaling the underlying infrastructure. Amazon ECR hosts your images in a highly available and scalable architecture, allowing you to reliably deploy containers for your applications. Integration with AWS Identity and Access Management (IAM) provides resource-level control of each repository. With Amazon ECR, there are no upfront fees or commitments. You pay only for the amount of data you store in your repositories and data transferred to the Internet.

## Decision Outcome

*   Amazon EKS
*   Amazon ECR
*   Terraform
*   GitLab CI-Runner
*   GitLab AutoDevops
