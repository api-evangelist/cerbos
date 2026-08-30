---
title: "Istio authorization stops at identity, not at what a workload may do"
url: "https://cerbos.dev/blog/istio-authorization-stops-at-identity"
date: "2026-08-24"
author: "Emre Baran"
feed_url: "https://www.cerbos.dev/rss/index.xml"
---
Istio proves which workload is calling with mTLS and SPIFFE, and stops there. This guide covers where AuthorizationPolicy runs out, handing the decision to an external authorizer through the CUSTOM action, running one policy set across north south and east west traffic, and what the extra network hops cost.
