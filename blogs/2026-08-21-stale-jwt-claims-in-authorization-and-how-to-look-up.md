---
title: "Stale JWT claims in authorization, and how to look up identity attributes at decision time"
url: "https://cerbos.dev/blog/how-to-look-up-identity-attributes-at-decision-time"
date: "2026-08-21"
author: "Alex Olivier"
feed_url: "https://www.cerbos.dev/rss/index.xml"
---
How to resolve identity attributes at decision time rather than reading stale JWT claims. Covers Envoy verifying the token while a Synapse data source fetches current profile and group data, policies that read attributes rather than claims, per source cache expiry, and failure behavior when the provider is unreachable.
