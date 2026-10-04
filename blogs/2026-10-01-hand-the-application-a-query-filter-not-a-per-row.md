---
title: "Hand the application a query filter, not a per row authorization decision"
url: "https://cerbos.dev/blog/hand-the-application-a-query-filter"
date: "2026-10-01"
author: "Alex Olivier"
feed_url: "https://www.cerbos.dev/rss/index.xml"
---
Per record authorization breaks when an application renders a list. This guide covers asking the policy engine what a user can see, turning a query plan into a database predicate, where AuthZEN search endpoints fit, and why translating to SQL, ORM or vector filters belongs in one place.
