# content-otaviorossoni.com

Content repository for [otaviorossoni.com](https://otaviorossoni.com).

## Structure

```
blog/
  pt/   # Portuguese posts
  en/   # English posts
  es/   # Spanish posts

projects/
  pt/   # Portuguese projects
  en/   # English projects
  es/   # Spanish projects
```

All posts are `.mdx` files named `yyyy-mm-dd-{slug}.mdx`. The slug stays the same across languages; only the directory changes.

```
blog/pt/2026-06-18-primeiro-post.mdx
blog/en/2026-06-18-first-post.mdx
```

## Frontmatter

Every post requires:

```yaml
---
title: ""
description: ""
date: "yyyy-mm-dd"
---
```

### Projects Frontmatter

Project files use a different frontmatter structure:

```yaml
---
title: ""
description: ""
href: ""
date: "yyyy-mm-dd"
duration: "Mon YYYY - Mon YYYY"
---
```

- `title` — project title
- `description` — short description
- `href` — link to the project repository or live site
- `date` — project date (used for ordering)
- `duration` — project duration with localized month names (use "Presente" for PT/ES, "Present" for EN for ongoing projects)
