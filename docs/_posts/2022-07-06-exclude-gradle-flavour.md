---
layout: post
title: Exclude Gradle Task
date: 2022-07-06 10:06 +0200
---

When building a multi-module project you might want to skip a task.
Usually it comes in handy when you dont want to `assemble` a specific module.

You can achieve it by specifying the excluded task:

```
./gradlew assembleRelease -x :app:assembleRelease
```

In the case above we are excluding the module `app` from building.

