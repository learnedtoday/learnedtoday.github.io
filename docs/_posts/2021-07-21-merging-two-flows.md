---
layout: post
title: "Merging two flows"
date: 2021-07-21 00:09:00 -0400
---
To merge two flows and achieve a result in which as values from any sequence are produced, those values become part of the result sequence.

Use the approach: 
`flowOf(flowA, flowB).flattenMerge()`


