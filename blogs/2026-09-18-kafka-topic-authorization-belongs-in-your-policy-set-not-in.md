---
title: "Kafka topic authorization belongs in your policy set, not in a per cluster ACL list"
url: "https://cerbos.dev/blog/kafka-topic-authorization-belongs-in-policy-set"
date: "2026-09-18"
author: "Alex Olivier"
feed_url: "https://www.cerbos.dev/rss/index.xml"
---
Kafka ACLs accumulate per cluster. This guide covers how Kafka's pluggable authorizer hands topic access decisions to an external policy engine, how ACL bindings map onto resource policies, caching and fail closed tradeoffs on the broker hot path, and what moves topic access into one audited policy set.
