# Triad Systems Website

A modern, professional website built with Hugo static site generator using the Tella theme.

## 🚀 Features

- ✨ **Modern Theme**: Built with the Tella Hugo theme for a professional look
- 📸 **Image Carousel**: Beautiful hero slider with custom AI-themed images
- 🎨 **Feature Cards**: Showcase services with icon-based feature sections
- 📝 **Blog**: Built-in blog functionality for sharing insights
- 🔒 **Secure**: Static site generation eliminates server-side vulnerabilities
- ⚡ **Fast**: Lightning-fast page loads with Tailwind CSS optimization
- 📱 **Responsive**: Beautiful design that works on all devices

## 📝 How to Update Content

### Quick Edit (Easiest Method)

1. **Edit content files** in `hugo-src/content/`:
   - `_index.md` - Homepage content (note: most homepage content is in data files)
   - `about.md` - About page
   - `solutions.md` - Solutions page
   - `contact.md` - Contact page
   - `blog/*.md` - Blog posts

2. **Update features and slides**:
   - `hugo-src/data/features.json` - Feature cards on homepage
   - `hugo-src/data/slide.json` - Hero slider configuration

3. **Rebuild the site**: The GitHub Actions workflow will automatically rebuild when you push changes to `hugo-src/`. Or manually run:
   ```bash
   hugo -s hugo-src
   ```

4. **Commit and push**:
   ```bash
   git add .
   git commit -m "Updated content"
   git push
   ```

## 🎨 Customization

### Update Site Configuration

Edit `hugo-src/config.toml` to change:
- Site title and description
- Navigation menu items
- Theme parameters
- Social media links

### Add/Change Images

- Logo: `hugo-src/static/img/logo/logo.svg`
- Slider images: `hugo-src/static/img/slide/`
- Blog post images: Add to `hugo-src/static/img/blog/`

### Modify Features

Edit `hugo-src/data/features.json` to change the feature cards on the homepage:
```json
{
  "title": "Feature Title",
  "description": "Feature description",
  "icon": "bi bi-icon-name"
}
```

## Markdown Formatting Guide

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
wget https://github.com/gohugoio/hugo/releases/download/v0.145.0/hugo_extended_0.145.0_Linux-64bit.tar.gz
tar -xzf hugo_extended_0.145.0_Linux-64bit.tar.gz
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
