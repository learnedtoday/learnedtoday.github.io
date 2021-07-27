---
layout: post
title: "The difference between StateFlow — SharedFlow — Channel"
date: 2021-07-20 00:010:00 -0400
---
With the shared flow, events are broadcast to an unknown number (zero or more) of subscribers. In the absence of a subscriber, any posted event is immediately dropped. It is a design pattern to use for events that must be processed immediately or not at all.

With the channel, each event is delivered to a single subscriber. An attempt to post an event without subscribers will be suspended as soon as the channel buffer becomes full, waiting for a subscriber to appear. Posted events are never dropped by default.

**Read More:** [Shared flows, broadcast channels by Roman Elizarov](https://elizarov.medium.com/shared-flows-broadcast-channels-899b675e805c)

