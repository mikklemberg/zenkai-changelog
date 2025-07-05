# Zenkai Changelog

Behind the line — Updates and improvements to Zenkai

## 🚀 How to Add New Entries

### 1. Create a New Markdown File

Create a new file in `_posts/` with the naming format: `YYYY-MM-DD-title.md`

Example: `_posts/2025-07-15-new-feature.md`

### 2. Add Front Matter

Start your file with front matter (the content between `---` lines):

```yaml
---
layout: entry
title: "Your Feature Title"
date: 2025-07-15
hero_text: "🎉 New Feature"  # Optional: for placeholder hero
image: "/assets/images/hero.jpg"  # Optional: for hero image
video_link: "https://youtube.com/watch?v=demo"  # Optional: demo video
excerpt: "Brief description of the update for the main page..."
---
```

### 3. Write Your Content

Write your changelog content in Markdown below the front matter:

```markdown
Your opening paragraph describing the main update...

## Major Feature Name

Description of the feature and why it matters.

## Another Feature

More details about improvements.

## Other improvements

- Bullet point improvement 1
- Bullet point improvement 2
- Bullet point improvement 3
```

### 4. Commit and Push

Once you commit and push to GitHub, Jekyll will automatically:
- Convert your markdown to HTML
- Generate individual pages with clean URLs
- Update the main changelog index
- Deploy to `changelog.zenkai.ee`

## 📁 File Structure

```
├── _config.yml          # Jekyll configuration
├── _layouts/
│   ├── default.html     # Base layout
│   └── entry.html       # Entry layout
├── _sass/
│   └── changelog.scss   # Styles
├── assets/
│   ├── css/main.scss    # Main stylesheet
│   └── images/          # Your images
├── _posts/              # Your markdown entries
│   └── 2025-07-05-zenkai-launch.md
├── index.html           # Main page
└── CNAME               # Custom domain
```

## 🎨 Customization

### Adding Images

1. Add images to `assets/images/`
2. Reference them in front matter: `image: "/assets/images/your-image.jpg"`

### Styling

- Main styles are in `_sass/changelog.scss`
- Uses CSS variables for easy customization
- Responsive design built-in

### URLs

- Main page: `changelog.zenkai.ee`
- Individual entries: `changelog.zenkai.ee/title-of-entry`

## 🔧 Local Development

To run locally:

1. Install Jekyll: `gem install jekyll bundler`
2. Run: `bundle exec jekyll serve`
3. Visit: `http://localhost:4000`

## 🌐 Deployment

GitHub Pages automatically builds and deploys when you push to the main branch.

## 📝 Front Matter Options

- `title`: Entry title (required)
- `date`: Publication date (required)
- `layout`: Should be "entry" (required)
- `hero_text`: Text for hero placeholder (optional)
- `image`: Hero image path (optional)
- `video_link`: Demo video URL (optional)
- `excerpt`: Brief description for main page (optional)

## 📋 Example Entry

See `_posts/2025-07-05-zenkai-launch.md` for a complete example.

## 🎯 Best Practices

1. **File naming**: Use `YYYY-MM-DD-descriptive-title.md`
2. **Excerpts**: Keep under 200 characters
3. **Images**: Optimize for web (under 1MB)
4. **Content**: Write naturally, no rigid structure required
5. **Dates**: Use ISO format (YYYY-MM-DD) in front matter
