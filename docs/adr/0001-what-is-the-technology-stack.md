# ADR 1: What is ReadyPitchGo's technology stack?

* Status: [proposed | rejected | accepted | deprecated | … | superseded by [ADR-0005](0005-example.md)] <!-- optional -->
* Deciders: [list everyone involved in the decision] <!-- optional -->
* Date: [YYYY-MM-DD when the decision was last updated] <!-- optional -->

Technical Story: 

**ReadyPitchGo** Is a (fictitious) Cie startup that Is tasked with creating a SaaS platform that will need to support every major league, minor league, collegiate and high school baseball teams. There are an estimated 40,000 teams each with 15 pitchers per year that will need to be monitored. This platform's main purpose Is to track the performance of a team's pitchers by tracking their velocity, the type of pitch and the effectiveness.
 
> PLEASE NOTE: The ReadyPitchGo team will have at least a few developers working on this platform at the same time, so please be cognizant of that when answering some of the questions defined below.
 
At the core of ReadyPitchGo are the following properties:
 
* A hardware component (pitch speed and type detection) that will log every pitch from every pitcher (type of pitch, speed of the pitch, whether the pitch was a ball or a strike) for each supported team
* Assume that the hardware component Is configured to hit a specific set of endpoints with configured team Information, pitcher and pitch Information
* An API or set of APIs for the hardware, reporting and various other properties to Interface with
* A reporting and team admin tool for the teams to login and view high level reports for:
* Their team: average velocity, pitch types, risky pitchers and other misc. self-service reports
* Metrics for each pitcher
* Modify their teams (add/edit/deactivate pitchers)
* Manage billing
	* A ReadyPitchGo admin tool to setup teams and view diagnostic Information
	* Scheduled tasks for billing and any reporting purposes
	* Underlying data storage Including caching, reporting, etc.
	* Any other properties determined by the technical team

> PLEASE NOTE: On the technical roadmap, there are plans for mobile applications that will also Interface with the API/APIs, however their functionality set and release date Is TBD.

## Context and Problem Statement

[Describe the context and problem statement, e.g., in free form using two to three sentences. You may want to articulate the problem in form of a question.]

## Decision Drivers <!-- optional -->

* [driver 1, e.g., a force, facing concern, …]
* [driver 2, e.g., a force, facing concern, …]
* … <!-- numbers of drivers can vary -->

## Considered Options

* [option 1]
* [option 2]
* [option 3]
* … <!-- numbers of options can vary -->

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
