---
layout: post
title: "Filter build variants"
date: 2021-07-23 00:09:00 -0400
---
Filter build variants by ignoring the flavour or buildType explicitly in the gradle file:

```
android{
    variantFilter { variant ->
	    // Filter Logic
    }
}
```

**Read More:** [Configure build variants](https://developer.android.com/studio/build/build-variants#workBuildVariants)

