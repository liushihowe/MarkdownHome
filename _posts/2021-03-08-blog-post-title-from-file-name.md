---
layout: post
title: "Blog Post Title From First Header"
date: 2021-03-08
---

<!--
    Post Front Matter 说明（中文注释）
    - title: 文章标题，会显示在页面和 meta 中
    - date: 文章日期，影响排序和 URL
    - author: 作者名字，可不设则使用 `_config.yml` 的默认作者
    - categories/tags: 用于分类和标签页的归档检索
    - description/excerpt: 列表或分享时的摘要文本
    - image: 可选的封面图路径
    - toc: 是否显示目录（如果主题支持）
    - comments: 是否允许评论
    编辑提示: 修改 front matter 后，保存并使用 `jekyll serve` 本地预览。
-->

### 这是一篇示例博客文章。您可以在这里讨论各种有趣的事情

---

### 支持语言高亮

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


print(f"斐波那契数列第 {10} 项是: {fibonacci(10)}")
```

### TypeScript 示例

```typescript
interface User {
    id: number;
    name: string;
    email: string;
}

function createUser(id: number, name: string, email: string): User {
    return { id, name, email };
}

const user = createUser(1, "someone", "abc@example.com");
console.log(user);
```
