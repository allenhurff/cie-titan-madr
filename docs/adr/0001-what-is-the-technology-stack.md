# ADR 1: What is the technology stack?

## Context and Problem Statement

*   What programming languages would you use for the API/APIs? Why?
*   Which database technology(ies) would you leverage? Why?
*   What other platforms would you leverage, if at all? Why?

## Considered Options

#### Programming Languages for APIs
*   [OpenAPI/Swagger 3.0](https://swagger.io/specification/) – It defines a standard, language-agnostic interface to RESTful APIs which allows both humans and computers to discover and understand the capabilities of the service without access to source code, documentation, or through network traffic inspection. OpenAPI Specification is a tool in the API Tools category of a tech stack.
*   [GraphQL](https://stackshare.io/graphql) – GraphQL is a data query language and runtime designed and used at Facebook to request and deliver data to mobile and web apps since 2012. GraphQL is a tool in the Query Languages category of a tech stack. GraphQL is an open source tool with 11.8K GitHub stars and 760 GitHub forks.

#### API Server/Cloud Technologies
*   [Kong](https://konghq.com/kong/) – Kong is a scalable, open source API Layer (also known as an API Gateway, or API Middleware). Kong controls layer 4 and 7 traffic and is extended through Plugins, which provide extra functionality and services beyond the core platform. Kong is a tool in the Microservices Tools category of a tech stack. Kong is an open source tool with 22.7K GitHub stars and 2.8K GitHub fork
*   [Amazon API Gateway](https://aws.amazon.com/api-gateway/) – Amazon API Gateway handles all the tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls, including traffic management, authorization and access control, monitoring, and API version management. Amazon API Gateway is a tool in the API Tools category of a tech stack.

#### Databases & Datastores
*   [CoachroachDB](https://adr.github.io/madr/) – A cloud-native SQL database for building global, scalable cloud services that survive disasters.
*   [Spanner](https://cloud.google.com/spanner/) – Cloud Spanner is the first scalable, enterprise-grade, globally-distributed, and strongly consistent database service built for the cloud specifically to combine the benefits of relational database structure with non-relational horizontal scale. This combination delivers high-performance transactions and strong consistency across rows, regions, and continents with an industry-leading 99.999% availability SLA, no planned downtime, and enterprise-grade security. Cloud Spanner revolutionizes database administration and management and makes application development more efficient.
*   [InfluxDB](https://en.wikipedia.org/wiki/InfluxDB) – InfluxDB is a scalable datastore for metrics, events, and real-time analytics. It has a built-in HTTP API so you don't have to write any server side code to get up and running.  InfluxDB is designed to be scalable, simple to install and manage, and fast to get data in and out.
*   [ProfaneDB](https://profanedb.gitlab.io/) – A Protocol Buffers database. ProfaneDB doesn't want to reinvent the wheel. It uses RocksDB for great performance, the simplest way possible.
*   [Amazon RDS](https://aws.amazon.com/rds/) – A managed relational database service for MySQL, PostgreSQL, MariaDB, Oracle BYOL, or SQL Server

#### Task processing
*   [AWS Lamda](https://aws.amazon.com/lambda/) AWS Lambda is a compute service that runs your code in response to events and automatically manages the underlying compute resources for you. You can use AWS Lambda to extend other AWS services with custom logic, or create your own back-end services that operate at AWS scale, performance, and security.
*   [Kafka](https://www.striim.com/solutions/kafka-real-time-integration-stream-processing/) Kafka is a distributed, partitioned, replicated commit log service. It provides the functionality of a messaging system, but with a unique design


#### Design Patterns
*   [Design by Contract (DbC)](https://en.wikipedia.org/wiki/Design_by_contract)  – Design by contract (DbC), also known as contract programming, programming by contract and design-by-contract programming, is an approach for designing software. It prescribes that software designers should define formal, precise and verifiable interface specifications for software components, which extend the ordinary definition of abstract data types with preconditions, postconditions and invariants. These specifications are referred to as "contracts", in accordance with a conceptual metaphor with the conditions and obligations of business contracts.

#### Metal Models
*   [Invert](https://seekingalpha.com/article/4040474-invert-always-invert) – Inverting a problem to find solutions is a concept I heard from Charlie Munger. Inspired by the mathematician Carl Jacobi, he said:
> Invert, always invert: Turn a situation or problem upside down. Look at it backward. What happens if all our plans go wrong? Where don't we want to go, and how do you get there? Instead of looking for success, make a list of how to fail instead - through sloth, envy, resentment, self-pity, entitlement, all the mental habits of self-defeat. Avoid these qualities and you will succeed. Tell me where I'm going to die, that is, so I don't go there.

## Decision Outcome

Chosen option:

*   Implicit assumptions should be made explicit.
  Design documentation is important to enable people understanding the decisions later on.
  See also [A rational design process: How and why to fake it](https://doi.org/10.1109/TSE.1986.6312940).
*   The MADR format is lean and fits our development style.
*   The MADR structure is comprehensible and facilitates usage & maintenance.
*   The MADR project is vivid.
*   Version 2.1.2 is the latest one available when starting to document ADRs.
