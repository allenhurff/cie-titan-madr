# ADR 10: Load/Performance Testing

## Context and Problem Statement

*   How will you be confident that the ReadyPitchGo platforms can handle the load from 40,000 teams, 600,000 pitchers with hundreds of millions of logged data points?
*   What Is your load and performance testing plan?

## Decision Drivers <!-- optional -->

* [driver 1, e.g., a force, facing concern, …]
* [driver 2, e.g., a force, facing concern, …]
* … <!-- numbers of drivers can vary -->

## Considered Options

*   [Chaos Engineering](https://en.wikipedia.org/wiki/Chaos_engineering) – is the discipline of experimenting on a software system in production in order to build confidence in the system's capability to withstand turbulent and unexpected conditions.
*   [jMeter](http://jmeter.apache.org/) – is open source software, a 100% pure Java application designed to load test functional behavior and measure performance. It was originally designed for testing Web Applications but has since expanded to other test functions.
*   [BlazeMeter](https://blazemeter.com/) – Run massively scalable, open source-based tests against all of your apps, from web and mobile apps to microservices and APIs. Write tests as code in domain specific language (DSL) to generate and instantly run JMeter™ tests without leaving your favorite application development tool. Use the same DSL to configure and launch tests using any major open source performance testing tool. Validate performance at every software delivery stage.

## Decision Outcome

*   Choas Engineering
*   BlazeMeter
