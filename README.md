# Portfolio Site

A Jekyll-based portfolio website optimized for GitHub Pages, featuring support for photos, videos, and Fusion 360 embeds.

## 🚀 Getting Started

### Local Development

1. Install Ruby and Bundler
2. Clone this repository
3. Run:
   ```bash
   bundle install
   bundle exec jekyll serve
   ```
4. Visit `http://localhost:4000`

### Deploy to GitHub Pages

1. Push this code to a GitHub repository
2. Go to Settings > Pages
3. Select "GitHub Actions" as source
4. Your site will be available at `https://yourusername.github.io/repository-name`

## 📁 Adding Content

### Projects

Create new project files in `_projects/`:

```markdown
---
title: Project Name
image: /assets/images/project-image.jpg
technologies: [Fusion 360, 3D Printing]
date: 2024-01-15
---

Your project content here...
```

### Images

- Add images to `assets/images/`
- Reference as `/assets/images/filename.jpg`

### Fusion 360 Embeds

```liquid
{% include fusion360.html src="your-fusion360-url" title="Model Name" %}
```

### Photo Galleries

```liquid
{% include gallery.html images=page.gallery %}
```

### Videos

```liquid
{% include video.html type="youtube" id="video-id" title="Video Title" %}
```

## 🎨 Customization

- Edit `_config.yml` for site settings
- Modify `assets/css/style.scss` for styling
- Update navigation in `_layouts/default.html`

## 📱 Features

- ✅ Responsive design
- ✅ Photo galleries with lightbox
- ✅ Video embeds (YouTube, Vimeo, local)
- ✅ Fusion 360 3D model embeds
- ✅ SEO optimized
- ✅ Fast loading with lazy images
- ✅ GitHub Pages compatible