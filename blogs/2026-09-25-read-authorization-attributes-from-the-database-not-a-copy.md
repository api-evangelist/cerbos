---
title: "Read authorization attributes from the database, not a copy"
url: "https://cerbos.dev/blog/read-authorization-attributes-from-the-database"
date: "2026-09-25"
author: "Alex Olivier"
feed_url: "https://www.cerbos.dev/rss/index.xml"
---
Authorization attributes like plan tier, team and clearance already live in a database. How Cerbos Synapse fetches them at decision time with a SQL data source and a Starlark proxy extension, how to set cache TTL per attribute, and how checks fail closed when the database is unreachable.
