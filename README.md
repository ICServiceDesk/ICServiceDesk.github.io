# SD Updates

This repository hosts the Service Desk updates website and RSS feed, which can be displayed in TDX desktop or used on digital signage.

## Writing Posts

### File Structure

- Add new posts to the `/docs/_posts` folder
- Filename format: `YYYY-MM-DD-Title.md`
- Example: `2025-03-14-Break-Achievements.md`

### Post Format

Each post must include Front Matter at the top of the file:

```yaml
---
layout: post
title: "Your Title"
date: YYYY-MM-DD
---
```

The Front Matter determines how the page is rendered on the published site/feed. For more information, see [Jekyll Front Matter](https://jekyllrb.com/docs/front-matter/).

### Adding Images

1. Place images in the `/docs/assets/images` directory
2. Reference images in your markdown using the following format:
   ```markdown
   ![alt text](/assets/images/your-image.png)
   ```
3. Supported image formats: PNG, JPG, JPEG, GIF

### Creating Static Pages

For important or perennial information, you can create a static page by adding a permalink to the Front Matter:

```yaml
---
layout: page
title: "Your Title"
permalink: /yourpage
---
```

### Best Practices

1. Use clear, descriptive titles
2. Include relevant images to enhance your content
3. Format your content with proper markdown syntax
4. Keep posts concise and focused
5. Use appropriate heading levels (h1, h2, h3) for structure

## Local Development

To test your changes locally:

1. Navigate to the `/docs` directory
2. Run `bundle install` to install dependencies
3. Run `bundle exec jekyll serve` to start the local server
4. View your site at `http://localhost:4000`

## Deployment

The site is automatically deployed to GitHub Pages when changes are pushed to the main branch.
