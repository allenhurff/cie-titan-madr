# ADR 0: ReadyPitchGo - Overview & Problem Statement

## Overview

**ReadyPitchGo** is a (fictitious) Cie startup that Is tasked with creating a SaaS platform that will need to support every major league, minor league, collegiate and high school baseball teams. There are an estimated 40,000 teams each with 15 pitchers per year that will need to be monitored. This platform's main purpose Is to track the performance of a team's pitchers by tracking their velocity, the type of pitch and the effectiveness.

## Problem Statement

> PLEASE NOTE: *The ReadyPitchGo team will have at least a few developers working on this platform at the same time, so please be cognizant of that when answering some of the questions defined below.*

At the core of ReadyPitchGo are the following properties:

*   A hardware component (pitch speed and type detection) that will log every pitch from every pitcher (type of pitch, speed of the pitch, whether the pitch was a ball or a strike) for each supported team
    *   *Assume that the hardware component Is configured to hit a specific set of endpoints with configured team Information, pitcher and pitch Information*
*   An API or set of APIs for the hardware, reporting and various other properties to Interface with
*   A reporting and team admin tool for the teams to login and view high level reports for:
    *   Their team: average velocity, pitch types, risky pitchers and other misc. self-service reports
    *   Metrics for each pitcher
    *   Modify their teams (add/edit/deactivate pitchers)
    *   Manage billing
*   A ReadyPitchGo admin tool to setup teams and view diagnostic Information
*   Scheduled tasks for billing and any reporting purposes
*   Underlying data storage Including caching, reporting, etc.
*   Any other properties determined by the technical team

> *PLEASE NOTE: On the technical roadmap, there are plans for mobile applications that will also Interface with the API/APIs, however their functionality set and release date Is TBD.*
