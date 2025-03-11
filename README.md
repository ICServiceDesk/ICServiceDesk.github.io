# SD

This exists to put an RSS feed in the TDX desktop or use the static pages on digital signage. Add posts to /docs/_posts folder. The posts must be formatted `YYYY-MM-DD-Title.md`. It is also best practice to add a layout to the page in markdown like:
```
---
layout: {post, page, home, base}
title: "Your title"
date: YYYY-MM-DD HH:MM:SS +/-TTTT
---
```

This box is called the [Front Matter](https://jekyllrb.com/docs/front-matter/) and determines how the page is reflected on the published site/feed.

For important or perennial news/information you can create a permalink in the Front Matter so that the site generates a static page and permanent link to that. That looks like this `permalink: /yourpage`