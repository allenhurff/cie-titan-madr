# ADR 8: Reporting

## Context and Problem Statement

*   What platforms/tools/approaches will you leverage to support ad-hoc, self-service reports for both teams and administrators?

## Decision Drivers <!-- optional -->

*   [Grafana vs. Kibana: The Key Differences to Know](https://logz.io/blog/grafana-vs-kibana/) – Kibana and Grafana are two popular open source tools that help users visualize and understand trends within vast amounts of log data, and in this post, I will give you a short introduction to each of the tools and highlight the key differences between them.
*   [Four Key Metrics] – (https://www.thoughtworks.com/radar/techniques/four-key-metrics) The researchers have determined that only four key metrics differentiate between low, medium and high performers: lead time, deployment frequency, mean time to restore (MTTR) and change fail percentage.

## Considered Options

*   [Grafana](https://grafana.com/) – is an open source visualization tool that can be used on top of a variety of different data stores but is most commonly used together with Graphite, InfluxDB, and also Elasticsearch and Logz.io.
*   [Prometheus](https://prometheus.io/docs/introduction/overview/) – Prometheus is an open-source systems monitoring and alerting toolkit originally built at SoundCloud. Since its inception in 2012, many companies and organizations have adopted Prometheus, and the project has a very active developer and user community. It is now a standalone open source project and maintained independently of any company.
*   [Graphite](https://en.wikipedia.org/wiki/Graphite_(software)) Graphite is a free open-source software (FOSS) tool that monitors and graphs numeric time-series data such as the performance of computer systems.
*   [Tableau](https://www.tableau.com/learn/webinars/introduction-tableau-server) – Tableau can help anyone see and understand their data. Connect to almost any database, drag and drop to create visualizations, and share with a click.
*   [Google Data Studio](https://datastudio.google.com/u/0/navigation/reporting) – Whether you’re looking to create detailed reports or high-level dashboards, Data Studio has the tools you need to easily bring your data analysis together, create compelling visualizations, and share insights with your team.

## Decision Outcome

*   Graphana
*   Tableau
