# 从零开始的 Jekyll 博客

这是一个基于 Jekyll 的静态博客项目，旨在帮助用户快速搭建个人博客。项目包含了 Jekyll 的基本配置、主题文件以及一些常用的功能扩展。

---

## 📂 项目结构

### 根目录

- **`_config.yml`**  
  Jekyll 的主配置文件，定义了站点的基本信息（如标题、描述、URL 等）以及插件、构建设置等。

- **`Gemfile` 和 `Gemfile.lock`**  
  用于管理 Ruby 的依赖项（如 Jekyll 和插件）。`Gemfile` 定义依赖，`Gemfile.lock` 锁定具体版本。

- **`README.md`**  
  当前文件，介绍项目的功能和文件结构。

---

### 📁 `_layouts/`

存放页面布局文件，定义了页面的整体结构。

- **`default.html`**  
  默认布局文件，包含了 `<head>` 和 `<body>` 的基本结构。

---

### 📁 `_includes/`

存放可复用的 HTML 片段。

- **`head.html`**  
  定义了页面的 `<head>` 部分，包括元数据和样式表的引用。
- **`header.html`**  
  定义了站点的头部导航栏。
- **`footer.html`**  
  定义了站点的底部信息。
- **`disqus_comments.html`**  
  集成 Disqus 评论系统的代码片段。

---

### 📁 `assets/`

存放静态资源文件，如 CSS、JS 和图片。

- **`assets/css/override.css`**  
  自定义的样式文件，用于覆盖默认主题的样式。
- **`assets/icons/`**  
  存放站点的图标文件（如 `favicon.ico`）。

---

### 📁 `_posts/`

存放博客文章的 Markdown 文件。文件命名格式为 `YYYY-MM-DD-title.md`。

---

### 📁 `_site/`

Jekyll 生成的静态文件目录，通常不需要手动修改。**注意：此目录不会被推送到 Git 仓库中（已在 `.gitignore` 中忽略）。**

---

### 📁 `_data/`

存放 YAML、JSON 或 CSV 格式的数据文件，可在模板中引用。

---

### 📁 `_plugins/`

存放自定义的 Jekyll 插件（Ruby 文件）。

---

## 🚀 快速开始

### 1. 安装依赖

确保已安装 Ruby 和 Bundler，然后运行以下命令安装依赖：

```bash
bundle install
```

### 2. 本地预览

运行以下命令启动本地开发服务器：

```bash
bundle exec jekyll serve --livereload
```

打开浏览器访问 [http://localhost:4000](http://localhost:4000)。

### 3. 部署到 GitHub Pages

将代码推送到 GitHub 仓库，并在仓库的 **Settings > Pages** 中启用 GitHub Pages。

---

## ✨ 功能特性

- **支持 Markdown**：使用简单的 Markdown 语法撰写文章。
- **自定义样式**：通过 `override.css` 文件轻松修改样式。
- **评论系统**：集成 Disqus 评论功能。
- **SEO 优化**：支持 `jekyll-seo-tag` 插件，自动生成元数据。
- **代码高亮**：支持代码块语法高亮。

---

## 📄 许可证

本项目遵循 MIT 许可证，详情请参阅 [LICENSE](LICENSE) 文件。
