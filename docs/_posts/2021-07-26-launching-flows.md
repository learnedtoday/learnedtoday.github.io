---
layout: post
title: "Launching Flows"
date: 2021-07-26 00:09:00 -0400
---
The *collect* keyword for a flow is a terminal operator on the coroutine context. Any subsequent operations won't be executed. 

One can work around by using a combination of *onEach* and *launchIn* operators.

**Read More:** [Launching Flows](https://kotlinlang.org/docs/flow.html#launching-flow)

