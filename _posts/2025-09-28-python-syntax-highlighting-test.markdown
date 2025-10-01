---
layout: post
title: "Python Syntax Highlighting Test"
date: 2025-09-28 14:30:00 +0800
categories: [test, highlight, python]
excerpt: "A short post to verify Python syntax highlighting on the site."
---

Below is a Python example that should be highlighted by the site's highlighter (Rouge by default):

```python
def greet(name: str) -> None:
    """Greet a user by name with a friendly message."""
    if not name:
        print("Hello, stranger!")
        return
    print(f"Hello, {name}!")

class Counter:
    def __init__(self):
        self.count = 0

    def inc(self):
        self.count += 1

if __name__ == '__main__':
    greet('Alice')
    c = Counter()
    for i in range(3):
        c.inc()
    print('count =', c.count)
```

If you see colored code tokens and line numbers (if enabled), the syntax highlighting works.
