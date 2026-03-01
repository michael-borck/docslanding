# Jekyll Documentation Theme

<!-- BADGES:START -->
[![dark-mode](https://img.shields.io/badge/-dark--mode-blue?style=flat-square)](https://github.com/topics/dark-mode) [![documentation](https://img.shields.io/badge/-documentation-blue?style=flat-square)](https://github.com/topics/documentation) [![github-pages](https://img.shields.io/badge/-github--pages-blue?style=flat-square)](https://github.com/topics/github-pages) [![jekyll](https://img.shields.io/badge/-jekyll-blue?style=flat-square)](https://github.com/topics/jekyll) [![landing-page](https://img.shields.io/badge/-landing--page-blue?style=flat-square)](https://github.com/topics/landing-page) [![responsive-design](https://img.shields.io/badge/-responsive--design-blue?style=flat-square)](https://github.com/topics/responsive-design) [![script-generation](https://img.shields.io/badge/-script--generation-blue?style=flat-square)](https://github.com/topics/script-generation) [![seo](https://img.shields.io/badge/-seo-blue?style=flat-square)](https://github.com/topics/seo) [![tailwind-css](https://img.shields.io/badge/-tailwind--css-blue?style=flat-square)](https://github.com/topics/tailwind-css) [![tool](https://img.shields.io/badge/-tool-607d8b?style=flat-square)](https://github.com/topics/tool)
<!-- BADGES:END -->

A beautiful, responsive Jekyll theme designed for **script-generated landing pages** + **automatic documentation**. Perfect for projects that generate landing pages from README.md and want integrated documentation.

## Features

- 🎨 **Modern Design**: Clean, professional look with Tailwind CSS
- 🌓 **Dark/Light Toggle**: Built-in theme switching
- 📱 **Responsive**: Mobile-friendly navigation and layout
- 🤖 **Script-Friendly**: Designed for automated landing page generation
- 📚 **Auto-Documentation**: Automatic navigation from folder structure
- ⚡ **Fast**: Optimized for GitHub Pages
- 🔍 **SEO Ready**: Built-in SEO optimization

## Quick Start

### 1. Add to your existing repository

Add this to your `_config.yml`:

```yaml
# Replace with your actual theme repository when published
remote_theme: your-username/jekyll-docs-theme

# Required settings
title: Your Project Name
description: Your project description
baseurl: "/your-repo-name"
url: "https://your-username.github.io"

# Author info
author:
  name: Your Name
  email: your-email@example.com

# GitHub info
github_username: your-username
repository: your-repo-name
```

### 2. Create your content structure

```
your-repo/
├── _config.yml
├── index.md                    # Landing page
├── docs/
│   ├── index.md               # Main documentation page
│   ├── getting-started/
│   │   ├── index.md
│   │   ├── installation.md
│   │   └── quick-start.md
│   ├── user-guide/
│   │   ├── index.md
│   │   └── ...
│   └── ...
```

### 3. Generate your landing page (`index.md`)

**For Script-Generated Content:**
Your script should:
1. Parse README.md for project information
2. Generate HTML content with Tailwind CSS classes
3. Create `index.md` with frontmatter + generated HTML:

```markdown
---
layout: default
title: Your Project Name  # From README
description: Your project description  # From README
---

<!-- Your script generates this HTML content from README.md -->
<section class="py-20 sm:py-24 lg:py-32">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8 text-center">
        <h1 class="text-4xl font-extrabold text-stone-900 dark:text-white">Project Name</h1>
        <!-- Generated buttons with fixed patterns -->
        <div class="mt-10 flex gap-4 justify-center">
            <a href="/docs/">Documentation</a>
            <a href="https://github.com/user/repo">GitHub</a>
            <a href="https://gitingest.com/user/repo">Ingest</a>
            <a href="https://deepwiki.com/user/repo">Deep Wiki</a>
        </div>
    </div>
</section>
<!-- More generated sections... -->
```

### 4. Enable GitHub Pages

1. Go to your repository settings
2. Navigate to "Pages"
3. Select "Deploy from a branch"
4. Choose `main` branch and `/ (root)` folder
5. Save

Your site will be available at `https://your-username.github.io/your-repo-name/`

## Customization

### Colors and Styling

The theme uses Tailwind CSS with a stone/sky color palette. You can customize by:

1. **Override CSS**: Create `assets/css/custom.css` and add to your layout
2. **Modify Tailwind config**: The theme includes custom color definitions
3. **Custom layouts**: Create your own layouts in `_layouts/`

### Navigation

Customize navigation in `_config.yml`:

```yaml
header_pages:
  - index.md
  - docs/your-section/index.md
  - docs/another-section/index.md
```

### Landing Page Sections

The theme provides flexible section layouts. Common patterns:

```html
<!-- Feature grid -->
<section class="py-16 sm:py-20 lg:py-24 bg-white dark:bg-stone-800">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
            <h2 class="text-3xl font-bold tracking-tight text-stone-900 dark:text-white sm:text-4xl">Features</h2>
        </div>
        <!-- Feature cards here -->
    </div>
</section>
```

## Documentation Structure

### Recommended folder structure:

```
docs/
├── index.md                    # Main docs page
├── getting-started/
│   ├── index.md               # Section overview
│   ├── installation.md
│   ├── quick-start.md
│   └── first-use.md
├── user-guide/
│   ├── index.md
│   ├── interface-overview.md
│   └── ...
├── features/
├── tutorials/
├── troubleshooting/
└── reference/
```

### Page frontmatter:

```yaml
---
layout: page
title: Page Title
description: Page description for SEO
---
```

## Development

### Local development:

```bash
# Install dependencies
bundle install

# Serve locally
bundle exec jekyll serve

# Build for production
bundle exec jekyll build
```

### Theme development:

If you want to modify the theme itself:

1. Fork this repository
2. Make your changes
3. Test with a sample site
4. Use as remote theme: `remote_theme: your-username/your-fork`

## Examples

Sites using this theme:
- [DeepTalk Documentation](https://michael-borck.github.io/deep-talk/)

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This theme is available as open source under the [MIT License](LICENSE).

## Support

- 🐛 **Issues**: [GitHub Issues](https://github.com/your-username/jekyll-docs-theme/issues)
- 💬 **Discussions**: [GitHub Discussions](https://github.com/your-username/jekyll-docs-theme/discussions)
- 📚 **Documentation**: This README and example site