# MarkdownHome

> Build Your Personal Site with Just Markdown - Zero Frontend Knowledge Required

MarkdownHome is a minimalist Jekyll theme designed for creators. All you need to know is Markdown to have a professional personal website and blog. No frontend skills needed, no worrying about styling - just focus on creating content.

## ✨ Features

- **🚀 Ready to Use** - Clone and go, no complex setup required
- **📝 Pure Markdown** - Write Markdown files, get beautiful pages automatically
- **🎨 Professional Design** - Carefully crafted responsive layout for all devices
- **📱 Completely Free** - Deploy on GitHub Pages at zero cost
- **⚡ Blazing Fast** - Static site, fast loading, SEO friendly

## 🚀 Quick Start

## 🚀 Quick Start (copy & use)

1. Click "Use this template" on GitHub or clone this repository to get started.
2. Edit `_config.yml` to set `title`, `description`, `url`, and any social links you want to show.
3. Add or edit pages (root) and posts (`_posts/`).
4. Commit and push to your repository; enable GitHub Pages in repository Settings to publish the site.

This repository is meant to be copied and used as-is. If you want to customize templates or styles, edit files in `_layouts/`, `_includes/`, and `_sass/`.

## 📁 Project Structure

```markdown
MarkdownHome/
├── _config.yml          # Site configuration file
├── _posts/              # Blog posts directory
│   └── 2024-01-15-welcome.md
├── about.md             # About page
├── index.md             # Home page
└── assets/              # Static assets
    └── css/
        └── style.scss   # Styles (no need to modify)
```

## 🎯 Usage Guide

### Writing New Posts

1. Create new files in the `_posts/` directory
2. Filename format: `year-month-day-post-title.md`
3. Add Front Matter at the top:

```markdown
---
layout: post
title: "Your Post Title"
date: 2024-01-15
categories: [diary, life]  # Optional categories
---
```

### Creating Custom Pages

Creating new pages is simple:

```markdown
---
layout: page
title: "Page Title"
---

Your page content...
```

### Adding Images

Place images in the `assets/images/` directory, then reference in your posts:

```markdown
![Image description](/assets/images/your-image.jpg)
```

## 🛠 Advanced Configuration

### Modifying Navigation Menu

Edit navigation configuration in `_config.yml`:

```yaml
header_pages:
  - about.md
  - your-custom-page.md
```

### Adding Comment System

Supports Disqus comments, configure in `_config.yml`:

```yaml
disqus:
  shortname: your-disqus-shortname
```

## ❓ Frequently Asked Questions

### Q: My site isn't updating?

A: GitHub Pages deployment takes a few minutes, please be patient.

### Q: How to modify site styling?

A: While the theme is designed to work without styling changes, advanced users can customize SCSS variables in the `_sass/` directory.

### Q: Does it support custom domains?

A: Yes! Create a `CNAME` file in the repository root with your domain name inside.

## 📚 Learning Resources

- [Jekyll Official Documentation](https://jekyllrb.com/)
- [Markdown Syntax Guide](https://www.markdownguide.org/)
- [GitHub Pages Help](https://docs.github.com/categories/github-pages-basics/)

## 🤝 Contributing

Issues and Pull Requests are welcome! If you have improvements or find bugs, please let us know.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Start your creation journey!** 🎉

If you have any questions, check [GitHub Issues](https://github.com/liushihowe/MarkdownHome/issues) or create a new Issue.
