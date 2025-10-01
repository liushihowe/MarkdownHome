---
layout: post
title: "博客模板功能完整展示"
date: 2025-10-01 12:00:00 +0800
categories: guide template
---

这篇文章展示了本博客模板的所有排版功能和样式效果，包括标题、段落、列表、代码高亮、表格、引用等。

---

## 1. 标题层级展示

### 三级标题样式

这是三级标题下的内容，字号为 24px，字重为 Medium (500)。

#### 四级标题样式

这是四级标题下的内容，字号为 20px，字重为 Regular (400)。

##### 五级标题样式

这是五级标题下的内容，字号为 16px。

###### 六级标题样式

这是六级标题下的内容，字号为 14px。

---

## 2. 文本样式

这是普通段落文本。本模板使用 HarmonyOS Sans 字体系统，行高为 1.65，确保良好的阅读体验。段落之间有 24px 的间距。

这是**粗体文本**，使用字重 700。这是*斜体文本*，用于强调。这是***粗斜体文本***，结合两者效果。

这是一个包含[超链接](https://github.com)的段落。悬停时链接会显示底部装饰线，颜色会加深。

---

## 3. 列表功能

### 无序列表

- 第一项：本模板支持多种 Markdown 语法
- 第二项：采用现代化设计风格
  - 嵌套项 1：支持列表嵌套
  - 嵌套项 2：间距合理
- 第三项：完整的响应式设计

### 有序列表

1. 第一步：克隆仓库到本地
2. 第二步：安装 Jekyll 依赖
3. 第三步：运行本地服务器
   1. 执行 `bundle install`
   2. 执行 `bundle exec jekyll serve`
4. 第四步：开始写作

### 任务列表

- [x] 完成 CSS 优化
- [x] 实现代码高亮
- [x] 优化表格样式
- [ ] 添加评论功能
- [ ] 集成搜索功能

---

## 4. 代码高亮展示

### 行内代码

在文本中使用 `inline code` 来表示代码片段，例如 `npm install` 或 `git commit`。行内代码有浅灰背景和细边框。

### Python 代码块

```python
# Python 示例：快速排序算法
def quicksort(arr):
    """
    快速排序实现
    时间复杂度：O(n log n)
    """
    if len(arr) <= 1:
        return arr
    
    pivot = arr[len(arr) // 2]
    left = [x for x in arr if x < pivot]
    middle = [x for x in arr if x == pivot]
    right = [x for x in arr if x > pivot]
    
    return quicksort(left) + middle + quicksort(right)

# 测试代码
numbers = [3, 6, 8, 10, 1, 2, 1]
sorted_numbers = quicksort(numbers)
print(f"排序结果: {sorted_numbers}")
```

### JavaScript 代码块

```javascript
// JavaScript 示例：异步数据获取
async function fetchUserData(userId) {
  try {
    const response = await fetch(`/api/users/${userId}`);
    
    if (!response.ok) {
      throw new Error(`HTTP error! status: ${response.status}`);
    }
    
    const data = await response.json();
    console.log('User data:', data);
    
    return data;
  } catch (error) {
    console.error('Error fetching user:', error);
    throw error;
  }
}

// 使用示例
fetchUserData(123)
  .then(user => console.log(user.name))
  .catch(err => console.error(err));
```

### HTML 代码块

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>示例页面</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header class="site-header">
    <h1>欢迎访问</h1>
    <nav>
      <a href="#home">首页</a>
      <a href="#about">关于</a>
    </nav>
  </header>
  
  <main class="content">
    <article>
      <h2>文章标题</h2>
      <p>这是文章内容...</p>
    </article>
  </main>
  
  <script src="script.js"></script>
</body>
</html>
```

### CSS 代码块

```css
/* 现代 CSS 变量系统 */
:root {
  --color-primary: #2563eb;
  --color-text: #1d1f23;
  --spacing-md: 24px;
  --radius-sm: 4px;
}

.card {
  background: white;
  border-radius: var(--radius-sm);
  padding: var(--spacing-md);
  box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  transition: transform 0.2s ease;
}

.card:hover {
  transform: translateY(-4px);
  box-shadow: 0 4px 16px rgba(0, 0, 0, 0.15);
}
```

### Bash 命令

```bash
# Git 常用命令
git init
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/username/repo.git
git push -u origin main

# Jekyll 本地运行
bundle install
bundle exec jekyll serve --livereload

# 部署到 GitHub Pages
git add .
git commit -m "Update content"
git push origin main
```

---

## 5. 表格展示

### 基础表格

| 功能 | 说明 | 状态 |
|------|------|------|
| 代码高亮 | 支持多语言语法高亮 | ✅ 完成 |
| 响应式设计 | 自适应各种屏幕尺寸 | ✅ 完成 |
| 暗色模式 | 护眼暗色主题 | ⏳ 进行中 |
| 评论系统 | 集成 Disqus/Giscus | 📝 计划中 |

### 复杂表格

| 编程语言 | 类型 | 难度 | 应用领域 | 推荐指数 |
|---------|------|------|----------|----------|
| Python | 解释型 | ⭐⭐⭐ | 数据科学、Web开发、自动化 | ⭐⭐⭐⭐⭐ |
| JavaScript | 解释型 | ⭐⭐⭐ | 前端开发、后端开发、移动应用 | ⭐⭐⭐⭐⭐ |
| Java | 编译型 | ⭐⭐⭐⭐ | 企业应用、Android开发 | ⭐⭐⭐⭐ |
| Go | 编译型 | ⭐⭐⭐ | 云服务、微服务、CLI工具 | ⭐⭐⭐⭐ |
| Rust | 编译型 | ⭐⭐⭐⭐⭐ | 系统编程、WebAssembly | ⭐⭐⭐⭐ |

### 代码对比表格

| 特性 | 传统方式 | 现代方式 |
|------|----------|----------|
| 变量 | `var x = 1;` | `const x = 1;` 或 `let y = 2;` |
| 函数 | `function fn() {}` | `const fn = () => {}` |
| 类 | `function Class() {}` | `class MyClass {}` |
| 异步 | `callback()` 或 `promise.then()` | `async/await` |

---

## 6. 引用块

### 普通引用

> 这是一个引用块。引用块使用左侧 4px 宽的蓝灰色边框，背景色为浅灰色，整体采用现代简洁风格。
>
> 引用块可以包含多个段落，字体颜色比正文略浅，非斜体显示以提高可读性。

### 嵌套引用

> 这是第一层引用。
>
> > 这是嵌套的第二层引用，可以用来表示引用中的引用。
> >
> > 嵌套引用同样保持良好的视觉层次。

### 包含代码的引用

> 在命令行中执行以下命令：
>
> ```bash
> npm install -g gatsby-cli
> gatsby new my-blog
> ```
>
> 这将创建一个新的 Gatsby 博客项目。

---

## 7. 分隔线

使用三个短横线创建分隔线：

---

分隔线在视觉上将内容分隔成不同的区块。

---

## 8. 图片展示

### 带说明的图片

![响应式设计示意图]({{ site.baseurl }}/assets/images/2025-10-01/responsive-design.jpg)
*图：响应式设计确保在各种设备上都有良好的显示效果*

---

## 9. 特殊格式

### 删除线

~~这段文字已被删除~~，使用两个波浪号包裹。

### 下标和上标

水的化学式是 H₂O，爱因斯坦的质能方程是 E=mc²。

### 脚注

这是一个包含脚注的句子[^1]。这是另一个脚注[^note]。

[^1]: 这是第一个脚注的内容。
[^note]: 这是一个命名脚注，可以使用有意义的标识符。

---

## 10. 定义列表

HTML
: 超文本标记语言，用于创建网页结构。

CSS
: 层叠样式表，用于控制网页外观和布局。

JavaScript
: 编程语言，为网页添加交互功能。

---

## 11. 数学公式支持

本模板使用 **MathJax 3** 渲染数学公式，支持 LaTeX 语法，提供清晰美观的数学表达式显示。**要不要试试点击公式放大和复制功能？**

### 行内公式

使用单个美元符号 `$...$` 包裹公式，可以在段落中嵌入数学表达式：

- 质能方程：$E = mc^2$
- 勾股定理：$a^2 + b^2 = c^2$
- 二次方程：$x = \frac{-b \pm \sqrt{b^2-4ac}}{2a}$
- 求和符号：$\sum_{i=1}^{n} i = \frac{n(n+1)}{2}$

在文本中使用很方便，例如：根据爱因斯坦的质能方程 $E = mc^2$，我们知道质量和能量是等价的。

### 块级公式

使用双美元符号 `$$...$$` 创建独立的公式块，公式会居中显示：

**组合数公式：**

$$
\frac{n!}{k!(n-k)!} = \binom{n}{k}
$$

**高斯积分：**

$$
\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}
$$

**矩阵表示：**

$$
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
\begin{bmatrix}
x \\
y
\end{bmatrix}
=
\begin{bmatrix}
ax + by \\
cx + dy
\end{bmatrix}
$$

**麦克斯韦方程组：**

$$
\begin{aligned}
\nabla \cdot \mathbf{E} &= \frac{\rho}{\epsilon_0} \\
\nabla \cdot \mathbf{B} &= 0 \\
\nabla \times \mathbf{E} &= -\frac{\partial \mathbf{B}}{\partial t} \\
\nabla \times \mathbf{B} &= \mu_0\mathbf{J} + \mu_0\epsilon_0\frac{\partial \mathbf{E}}{\partial t}
\end{aligned}
$$

### 交互功能

本模板的公式支持以下交互功能：

1. **点击放大** 📋  
   点击任意公式，会弹出放大窗口，方便查看复杂公式的细节

2. **一键复制** ✨  
   在放大窗口中点击"📋 复制公式"按钮，可以快速复制公式文本

3. **统一配色** 🎨  
   公式窗口采用与代码块相同的配色方案，视觉风格统一

### 常用 LaTeX 语法示例

**上标和下标：**

- 上标：`x^2` → $x^2$
- 下标：`x_i` → $x_i$
- 组合：`x_i^2` → $x_i^2$

**分数：**

- `\frac{a}{b}` → $\frac{a}{b}$
- `\dfrac{a}{b}` → $\dfrac{a}{b}$ (displaystyle)

**根式：**

- `\sqrt{x}` → $\sqrt{x}$
- `\sqrt[n]{x}` → $\sqrt[n]{x}$

**求和与积分：**

- `\sum_{i=1}^{n}` → $\sum_{i=1}^{n}$
- `\int_{a}^{b}` → $\int_{a}^{b}$
- `\prod_{i=1}^{n}` → $\prod_{i=1}^{n}$

**希腊字母：**

- `\alpha, \beta, \gamma` → $\alpha, \beta, \gamma$
- `\Delta, \Sigma, \Omega` → $\Delta, \Sigma, \Omega$

**特殊符号：**

- `\infty` → $\infty$
- `\partial` → $\partial$
- `\nabla` → $\nabla$
- `\pm` → $\pm$
- `\times` → $\times$
- `\cdot` → $\cdot$

**箭头：**

- `\rightarrow` → $\rightarrow$
- `\Rightarrow` → $\Rightarrow$
- `\leftrightarrow` → $\leftrightarrow$

---

## 12. Emoji 支持

本模板支持 Emoji 表情符号：

- 😀 开心
- 🎉 庆祝
- 💻 编程
- 📚 学习
- ✅ 完成
- ❌ 错误
- ⚠️ 警告
- 💡 想法
- 🚀 发布
- 🔥 热门

---

## 13. 特殊块元素

### 提示框（使用引用变体）

> **💡 提示**
>
> 这是一个提示信息，用于给读者提供额外的建议或说明。
> **⚠️ 警告**
>
> 这是一个警告信息，用于提醒读者注意潜在的问题或风险。
> **❌ 错误**
>
> 这是一个错误信息，表示某个操作失败或遇到问题。
> **✅ 成功**
>
> 这是一个成功信息，表示操作已成功完成。

---

## 14. 水平对齐

### 左对齐（默认）

这是左对齐的文本内容。

### 居中对齐

<div style="text-align: center;">
这是居中对齐的文本内容。
</div>

### 右对齐

<div style="text-align: right;">
这是右对齐的文本内容。
</div>

---

## 15. 缩写

HTML、CSS 和 JS 是前端开发的三大基础技术。

*[HTML]: HyperText Markup Language
*[CSS]: Cascading Style Sheets
*[JS]: JavaScript

---

## 总结

本文展示了博客模板的所有主要功能和样式效果。模板采用现代化设计，具有以下特点：

1. ✨ **优雅的排版** - 合理的字号、行高、间距系统
2. 🎨 **卡片式设计** - 表格、代码块采用卡片风格
3. 🌈 **精美的代码高亮** - 基于 One Light 配色方案
4. 📱 **完全响应式** - 适配手机、平板、桌面端
5. ⚡ **流畅的交互** - 悬停动画、过渡效果
6. 🎯 **清晰的层次** - 标题、段落、列表结构分明
7. 💎 **细节优化** - 圆角、阴影、边框精心调校

欢迎使用本模板创作您的内容！如有问题或建议，欢迎反馈。

---

**文章标签：** `#模板` `#功能展示` `#Markdown` `#Jekyll`

**相关链接：**

- [GitHub 仓库](https://github.com)
- [Jekyll 文档](https://jekyllrb.com)
- [Markdown 指南](https://www.markdownguide.org)
