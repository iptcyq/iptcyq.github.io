### Github Page
Just a Github Page because I was bored in the middle of exam season.

---
### Adding New Project Pages

1. Create a new markdown file in `pages/`.
2. Add frontmatter like this at the top:

```md
---
title: Your Project Title
date: 2026-08-03
summary: One-line summary for homepage.
thumbnail: /images/your-image.png?raw=true
badge: Optional Label
external_url: https://example.com
home_post: true
---
```

3. Write your page content below it.
4. The page will automatically show up under "Project Log" on the homepage.

### Posts without a dedicated page:

1. Edit `_data/home_posts.yml`.
2. Add an item under `wip:` or `archive:` with fields like:

```yml
- title: Example Project
	date: 2026-08-03
	summary: Short summary text.
	thumbnail: /images/example.png?raw=true
	external_url: https://example.com
	external_label: External link
```

3. Leave out `page_url` if there is no dedicated page.

---
### References and Credits

[1] Jekyll theme "Minimal" for GitHub Pages: https://github.com/pages-themes/minimal (CC0 1.0 Universal License)
[2] Page template forked from evanca: https://github.com/evanca/quick-portfolio (Unlicense license)
