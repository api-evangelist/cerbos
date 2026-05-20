---
title: "From maps to bitmaps (and from bitmaps to bitmaps)"
url: "https://cerbos.dev/blog/from-maps-to-bitmaps-and-from-bitmaps-to-bitmaps"
date: "Wed, 13 May 2026 12:47:17 GMT"
author: "Sam Lock"
feed_url: "https://www.cerbos.dev/rss/"
---
Inside the Cerbos PDP performance rewrite that took authorization decisions from 43.8 µs to 6.6 µs. This post walks through three iterations of the rule table index, why roaring bitmaps weren't the right fit, and how a custom bitmap with a meta layer beat both the previous index and roaring.
