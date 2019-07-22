# ADR 12: Branching Strategy

## Context and Problem Statement

*   With so many features/functionality being developed concurrently, what branching strategy will you leverage?

## Decision Drivers <!-- optional -->



## Considered Options

*   [Feature Flag Development](https://en.wikipedia.org/wiki/Feature_toggle) – A feature toggle (also feature switch, feature flag, feature flipper, conditional feature, etc.) is a technique in software development that attempts to provide an alternative to maintaining multiple source-code branches (known as feature branches), such that a feature can be tested even before it is completed and ready for release. Feature toggle is used to hide, enable or disable the feature during run time. For example, during the development process, a developer can enable the feature for testing and disable it for other users.
*   [Trunk Based Development](https://trunkbaseddevelopment.com/) – A source-control branching model, where developers collaborate on code in a single branch called ‘trunk’ *, resist any pressure to create other long-lived development branches by employing documented techniques. They therefore avoid merge hell, do not break the build, and live happily ever after.

## Decision Outcome

*   Single Trunk, Feature Flag, Continous Deployment to Blue/Green/Grey
