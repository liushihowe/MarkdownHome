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

### Step 1: Create Your Repository

1. Visit [MarkdownHome GitHub Repository](https://github.com/liushihowe/MarkdownHome)
2. Click "Use this template" → "Create a new repository" in the top-right corner
3. Name your repository, suggested format: `yourusername.github.io`
   - Example: `johnsmith.github.io`

### Step 2: Basic Configuration

Open the `_config.yml` file and modify these basic settings:

```yaml
# Basic site information
title: "Your Site Title"
author: "Your Name"
description: "Site description"
baseurl: "" # Keep empty if repository name is username.github.io
url: "https://yourusername.github.io" # Your website URL

# Social links (optional)
github_username: your-github-username
twitter_username: your-twitter-username
email: your-email@example.com
```

### Step 3: Add Your Content

#### Create About Page

Create `about.md` in the root directory:

```markdown
---
layout: page
title: About Me
---

Write your self-introduction using Markdown here...
```

#### Write Blog Posts

Create posts in the `_posts/` directory with filename format: `year-month-day-title.md`

```markdown
---
layout: post
title: "My First Post"
date: 2024-01-15
---

Your post content here, written in **Markdown** syntax...
```

### Step 4: Deploy Your Site

1. Commit your changes to GitHub
2. Go to repository Settings → Pages
3. Ensure GitHub Pages source is set to "Deploy from a branch", select `main` or `master` branch
4. Wait a few minutes, then visit `https://yourusername.github.io` to see your live website!

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

- [Jekyll Official Documentation](https://jekyllrb.com/){:target="_blank" rel="noopener"}
- [Markdown Syntax Guide](https://www.markdownguide.org/){:target="_blank" rel="noopener"}
- [GitHub Pages Help](https://docs.github.com/categories/github-pages-basics/){:target="_blank" rel="noopener"}

## 🤝 Contributing

Issues and Pull Requests are welcome! If you have improvements or find bugs, please let us know.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Start your creation journey!** 🎉

If you have any questions, check [GitHub Issues](https://github.com/liushihowe/MarkdownHome/issues){:target="_blank" rel="noopener"} or create a new Issue.
