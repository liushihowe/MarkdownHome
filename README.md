# MarkdownHome

> 用 Markdown，建个人站 - 零前端知识，专注你的内容

MarkdownHome 是一个基于 Jekyll 的极简主题，专为创作者设计。你只需要会写 Markdown，就能拥有一个专业的个人网站和博客。无需任何前端知识，无需担心样式设计，专注于创作本身。

## ✨ 特性

- **🚀 开箱即用** - 克隆即用，无需配置复杂环境
- **📝 纯 Markdown** - 只需编写 Markdown 文件，自动生成美观页面
- **🎨 专业设计** - 精心设计的响应式布局，适配所有设备
- **📱 完全免费** - 基于 GitHub Pages，零成本部署
- **⚡ 极速体验** - 静态网站，加载速度快，SEO 友好

## 🚀 快速开始

### 第一步：创建你的仓库

1. 访问 [MarkdownHome GitHub 仓库](https://github.com/liushihowe/MarkdownHome)
2. 点击右上角的 "Use this template" → "Create a new repository"
3. 命名你的仓库，格式建议：`你的用户名.github.io`
   - 例如：`johnsmith.github.io`

### 第二步：基础配置

打开 `_config.yml` 文件，修改以下基本信息：

```yaml
# 站点基本信息
title: "你的网站标题"
author: "你的名字"
description: "网站描述"
baseurl: "" # 如果仓库名是 用户名.github.io，保持为空
url: "https://你的用户名.github.io" # 你的网站地址

# 社交链接（可选）
github_username: 你的GitHub用户名
twitter_username: 你的Twitter用户名
email: your-email@example.com
```

### 第三步：添加你的内容

#### 创建关于页面

在根目录创建 `about.md`：

```markdown
---
layout: page
title: 关于我
---

这里用 Markdown 写你的自我介绍...
```

#### 撰写博客文章

在 `_posts/` 目录下创建文章，文件名格式：`年-月-日-标题.md`

```markdown
---
layout: post
title: "我的第一篇文章"
date: 2024-01-15
---

这里是你的文章内容，使用 **Markdown** 语法编写...
```

### 第四步：部署网站

1. 提交你的更改到 GitHub
2. 进入仓库设置 → Pages
3. 确保 GitHub Pages 源设置为 "Deploy from a branch"，分支选择 `main` 或 `master`
4. 等待几分钟，访问 `https://你的用户名.github.io` 查看你的网站！

## 📁 项目结构

```markdown
MarkdownHome/
├── _config.yml          # 站点配置文件
├── _posts/              # 博客文章目录
│   └── 2024-01-15-welcome.md
├── about.md             # 关于页面
├── index.md             # 首页
└── assets/              # 静态资源
    └── css/
        └── style.scss   # 样式文件（无需修改）
```

## 🎯 使用指南

### 编写新文章

1. 在 `_posts/` 目录创建新文件
2. 文件名格式：`年-月-日-文章标题.md`
3. 文件开头添加 Front Matter：

```markdown
---
layout: post
title: "你的文章标题"
date: 2024-01-15
categories: [日记, 生活]  # 可选分类
---
```

### 自定义页面

创建任何新页面都很简单：

```markdown
---
layout: page
title: "页面标题"
---

你的页面内容...
```

### 添加图片

将图片放入 `assets/images/` 目录，然后在文章中引用：

```markdown
![图片描述](/assets/images/your-image.jpg)
```

## 🛠 高级配置

### 修改导航菜单

编辑 `_config.yml` 中的导航配置：

```yaml
header_pages:
  - about.md
  - your-custom-page.md
```

### 添加评论系统

支持 Disqus 评论，在 `_config.yml` 中配置：

```yaml
disqus:
  shortname: your-disqus-shortname
```

## ❓ 常见问题

### Q: 我的网站没有更新？

A: GitHub Pages 部署需要几分钟时间，请耐心等待。

### Q: 如何修改网站样式？

A: 虽然主题设计为无需修改样式，但高级用户可以在 `_sass/` 目录下自定义 SCSS 变量。

### Q: 支持自定义域名吗？

A: 支持！在仓库根目录创建 `CNAME` 文件，里面写入你的域名。

## 📚 学习资源

- [Jekyll 官方文档](https://jekyllrb.com/)
- [Markdown 语法指南](https://www.markdownguide.org/)
- [GitHub Pages 帮助](https://docs.github.com/categories/github-pages-basics/)

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！如果你有改进建议或发现了 bug，请告诉我们。

## 📄 许可证

本项目采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件。

---

**开始你的创作之旅吧！** 🎉

如果有任何问题，请查看 [GitHub Issues](https://github.com/liushihowe/MarkdownHome/issues) 或创建新的 Issue。
