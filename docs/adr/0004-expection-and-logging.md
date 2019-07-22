# ADR 4: Exception & Logging Handlings

## Context and Problem Statement

*   What frameworks/tooling will you leverage for exception logging?
*   Standard logging?

## Decision Drivers <!-- optional -->

*   Anything that goes STDERR & STDOUT!

## Considered Options

*   [ELK Stack](https://www.elastic.co/what-is/elk-stack) - "ELK" is the acronym for three open source projects: Elasticsearch, Logstash, and Kibana. Elasticsearch is a search and analytics engine. Logstash is a server‑side data processing pipeline that ingests data from multiple sources simultaneously, transforms it, and then sends it to a "stash" like Elasticsearch. Kibana lets users visualize data with charts and graphs in Elasticsearch.
*   [TICK Stack](https://www.thoughtworks.com/radar/platforms/tick-stack) - "TICK" Stack is a collection of open source components that combine to deliver a platform for easily storing, visualizing and monitoring time series data such as metrics and events. The components are: Telegraf, a server agent for collecting and reporting metrics; InfluxDB, a high-performance time series database; Chronograf, a user interface for the platform; and Kapacitor, a data-processing engine that can process, stream and batch data from InfluxDB. Unlike Prometheus, which is based on the pull model, TICK Stack is based on the push model of collecting data. The heart of the system is the InfluxDB component, which is one of the best time series databases. The stack is backed by InfluxData and although you need the enterprise version for features such as database clustering, it's still a fairly good choice for monitoring. We're using it in a few places in production and have had good experiences with it.
*   [Amazon CloudWatch](https://aws.amazon.com/cloudwatch/) - Amazon CloudWatch is a monitoring and management service built for developers, system operators, site reliability engineers (SRE), and IT managers. CloudWatch provides you with data and actionable insights to monitor your applications, understand and respond to system-wide performance changes, optimize resource utilization, and get a unified view of operational health. CloudWatch collects monitoring and operational data in the form of logs, metrics, and events, providing you with a unified view of AWS resources, applications and services that run on AWS, and on-premises servers.

## Decision Outcome

*   ELK stack
*   Amazon Cloud Watch
