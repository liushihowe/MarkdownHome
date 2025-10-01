---
layout: post
title: "测试：语法高亮效果"
date: 2025-09-26 12:00:00 +0800
---

### Python 示例

```python
def fibonacci(n: int) -> int:
    """返回斐波那契数列的第 n 项"""
    if n <= 1:
        return n
    a, b = 0, 1
    for _ in range(2, n + 1):
        a, b = b, a + b
    return b

print(f"fibonacci(10) = {fibonacci(10)}")
```

### 纯文本（txt）示例

```text
这是一个纯文本示例：
Line 1: Hello
Line 2: 这是中文行
Line 3: 12345
```

### 命令行 / 终端 示例（bash / console）

```bash
# 更新依赖并运行本地预览（示例）
bundle install
bundle exec jekyll serve --livereload

# 查看本地服务器输出：
# 在浏览器打开 http://127.0.0.1:4000
```

测试说明：如果你使用的是 highlight.js，请确保已正确把 `js/highlightjs/` 放到仓库并在 `_includes/head.html` 中引用本地或 CDN 文件；页面加载后应看到彩色高亮。若使用 Rouge，请在本地构建时查看生成的 HTML。
