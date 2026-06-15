---
title: "The Meta AI hack shows why agents shouldn't decide access"
url: "https://www.cerbos.dev/blog/meta-ai-hack-shows-why-agents-shouldnt-decide-access"
date: "2026-06-03"
author: "Emre Baran"
feed_url: "https://www.cerbos.dev/blog"
---
An attacker manipulated Instagram's AI support chatbot into granting unauthorized access to accounts by requesting the bot add a new email address, using a VPN to bypass location verification — resulting in password resets for high-profile accounts including those associated with the Obama-era White House and a U.S. Space Force official. The incident exposes two failures: authentication that did not verify actual account ownership, and an agent making access control decisions through a conversational interface where a language model can be persuaded through dialogue. Cerbos argues the solution is architectural: authorization decisions must reside outside the agent, evaluated against policies it cannot override.
