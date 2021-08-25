---
layout: post
title: Kotlin String Literals
date: 2021-08-25 14:06 +0200
---

Kotlin has two types of string literals:
- escaped strings that may contain escaped characters
- raw strings that can contain newlines and arbitrary text

Escaping is done in the conventional way, with a backslash (`\`).
```
val s = "Hello, world!\n"
```

A raw string is delimited by a triple quote (`"""`), contains no escaping and can contain newlines and any other characters:
```
val text = """
    for (c in "foo")
        print(c)
"""
```

