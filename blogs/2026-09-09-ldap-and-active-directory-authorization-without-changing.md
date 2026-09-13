---
title: "LDAP and Active Directory authorization without changing the application"
url: "https://cerbos.dev/blog/ldap-active-directory-authorization-without-changing-application"
date: "2026-09-09"
author: "Alex Olivier"
feed_url: "https://www.cerbos.dev/rss/index.xml"
---
LDAP and Active Directory groups encode the access rules for applications nobody will fund a rewrite for. Covers resolving those groups at the proxy in front of the application, turning them into an input to policy rather than the access model itself, cache staleness, and where boundary enforcement stops.
