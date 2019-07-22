# ADR 2: Caching Strategy

## Context and Problem Statement

*   What data can/should be cached?
*   What caching frameworks/platforms/approaches would you leverage and In what circumstances?

## Decision Drivers <!-- optional -->

*   [GraphQL vs REST: Caching](https://apisyouwonthate.com/blog/graphql-vs-rest-caching) – Comparing how caching is used for the two approaches is tricky, because despite common opinion, REST has nothing to do with HTTP. REST is usually implemented in HTTP, therefore when most folks talk about “caching in REST”, they are really talking about caching with HTTP. That is a huge topic in its own right.

## Considered Options

#### Caching for HTTP/APIs
*   [GraphQL Caching](https://graphql.org/learn/caching/) – In an endpoint-based API, clients can use HTTP caching to easily avoid refetching resources, and for identifying when two resources are the same. The URL in these APIs is a globally unique identifier that the client can leverage to build a cache. In GraphQL, though, there's no URL-like primitive that provides this globally unique identifier for a given object. It's hence a best practice for the API to expose such an identifier for clients to use.
*   [Varnish Caching](https://varnish-cache.org/) – Varnish Cache is a web application accelerator also known as a caching HTTP reverse proxy. You install it in front of any server that speaks HTTP and configure it to cache the contents. Varnish Cache is really, really fast. It typically speeds up delivery with a factor of 300 - 1000x, depending on your architecture.
*   [Amazon ElastiCache](https://aws.amazon.com/elasticache) - Amazon ElastiCache offers fully managed Redis and Memcached. Seamlessly deploy, run, and scale popular open source compatible in-memory data stores. Build data-intensive apps or improve the performance of your existing apps by retrieving data from high throughput and low latency in-memory data stores.

## Decision Outcome

Chosen option: "[option 1]", because [justification. e.g., only option, which meets k.o. criterion decision driver | which resolves force force | … | comes out best (see below)].
