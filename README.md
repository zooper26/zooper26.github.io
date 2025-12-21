# Triad Systems Website

A modern, secure, and easy-to-update landing page built with Hugo static site generator.

## 🚀 Features

- ✨ **Easy Editing**: Update content using simple Markdown - no HTML knowledge required!
- 🔒 **Secure**: Static site generation eliminates server-side vulnerabilities
- ⚡ **Fast**: Lightning-fast page loads with optimized static HTML
- 📱 **Responsive**: Beautiful design that works on all devices
- 🎨 **Customizable**: Easy to modify both content and design

## 📝 How to Update Content

### Quick Edit (Easiest Method)

1. **Edit the main content file**: `hugo-src/content/_index.md`
   - This file uses Markdown format
   - Simple syntax like `**bold**`, `*italic*`, `- bullet points`
   - No HTML knowledge needed!

2. **Rebuild the site**: Run this command from the repository root:
   ```bash
   ./hugo -s hugo-src
   ```

3. **Commit and push**:
   ```bash
   git add .
   git commit -m "Updated content"
   git push
   ```

### Markdown Formatting Guide

Here are some common Markdown formatting examples:

```markdown
# Heading 1
## Heading 2
### Heading 3

**Bold text**
*Italic text*
`Code or technical terms`

- Bullet point 1
- Bullet point 2
- Bullet point 3

1. Numbered item 1
2. Numbered item 2
3. Numbered item 3

[Link text](https://example.com)

---

Horizontal line above
```

## 🎨 Customization Options

### Change Site Title and Description

Edit `hugo-src/config.toml`:
```toml
title = "Your Site Name"

[params]
  description = "Your site description"
```

### Modify Design

Edit the template file at `hugo-src/layouts/index.html` to change:
- Colors (search for color codes like `#667eea`)
- Fonts (modify `font-family` values)
- Layout structure

### Add More Pages

1. Create new Markdown files in `hugo-src/content/`
2. Add frontmatter at the top:
   ```markdown
   ---
   title: "Page Title"
   date: 2024-12-21
   draft: false
   ---
   
   Your content here...
   ```

## 🔒 Security Features

- **Content Security Policy (CSP)**: Prevents XSS attacks
- **Static Generation**: No server-side code execution vulnerabilities
- **No Database**: Eliminates SQL injection risks
- **HTTPS Ready**: Works seamlessly with GitHub Pages HTTPS

## 📦 Project Structure

```
zooper26.github.io/
├── hugo-src/              # Hugo source files
│   ├── config.toml        # Site configuration
│   ├── content/           # Markdown content files
│   │   └── _index.md      # Main page content (EDIT THIS!)
│   ├── layouts/           # HTML templates
│   │   └── index.html     # Main template
│   └── static/            # Static assets (images, etc.)
├── index.html             # Generated homepage (don't edit directly)
├── sitemap.xml            # Generated sitemap
└── .nojekyll              # Tells GitHub Pages not to use Jekyll
```

## 🛠️ Setup Hugo (First Time Only)

If you need to install Hugo on a new machine:

### Linux/macOS:
```bash
wget https://github.com/gohugoio/hugo/releases/download/v0.121.1/hugo_extended_0.121.1_Linux-64bit.tar.gz
tar -xzf hugo_extended_0.121.1_Linux-64bit.tar.gz
chmod +x hugo
```

### Or use package managers:
```bash
# macOS
brew install hugo

# Ubuntu/Debian
sudo apt install hugo

# Windows (with Chocolatey)
choco install hugo-extended
```

## 📚 Additional Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [Markdown Guide](https://www.markdownguide.org/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

## 🤝 Contributing

To suggest improvements:
1. Edit the content or templates
2. Test locally by running `./hugo -s hugo-src`
3. Open your browser to `index.html` to preview
4. Commit and push your changes

## 📄 License

This website is for Triad Systems. Feel free to use the structure as a template for your own sites.

---

**Built with ❤️ using Hugo Static Site Generator**
