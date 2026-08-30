---
title: "Envoy ext_authz: enforcing one authorization policy at the gateway and in the service"
url: "https://cerbos.dev/blog/envoy-ext-authz-enforcing-one-authorization-policy-at-gateway-in-service"
date: "2026-08-14"
author: "Alex Olivier"
feed_url: "https://www.cerbos.dev/rss/index.xml"
---
Envoy external authorization with the ext_authz filter lets the gateway and the service run checks against one policy set. This guide covers the CheckRequest to Cerbos mapping in CEL, policy outputs as request headers, embedded versus external PDP, bypass paths, caching trade offs and what AuthZEN leaves undefined.
