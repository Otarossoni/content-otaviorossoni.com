# AGENTS.md

## Repository Purpose

This repository stores the content for [otaviorossoni.com](https://otaviorossoni.com) — a multilingual blog with posts in Portuguese (`pt/`), English (`en/`), and Spanish (`es/`).

## Directory Structure

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

## File Naming Convention

All blog post files **must** follow this naming pattern:

```
yyyy-mm-dd-{slug}
```

- `yyyy-mm-dd` — publication date (e.g., `2026-06-18`)
- `{slug}` — a short, lowercase, hyphenated identifier for the post (e.g., `introducao-ao-react`)

The same `{slug}` is used across all languages. The only difference between language versions is the directory (`pt/`, `en/`, `es/`).

Example:

```
blog/pt/2026-06-18-primeiro-post.mdx
blog/en/2026-06-18-first-post.mdx    # NOT the same slug
```

## Required Frontmatter

Every post **must** begin with this YAML frontmatter:

```yaml
---
title: ""
description: ""
date: "yyyy-mm-dd"
---
```

- `title` — post title
- `description` — short description (used for SEO/meta)
- `date` — publication date, must match the date in the filename

### Projects Frontmatter

Project files use a different frontmatter structure:

```yaml
---
title: ""
description: ""
href: ""
date: "yyyy-mm-dd"
duration: "Mon YYYY - Mon YYYY"
tags: "#tag1 #tag2 #tag3"
highlight: true/false
---
```

- `title` — project title
- `description` — short description (used for SEO/meta)
- `href` — link to the project repository or live site
- `date` — project date (used for ordering)
- `duration` — project duration in `{month/year start} - {month/year end}` format, with month names localized per language (use "Presente" for PT/ES, "Present" for EN for ongoing projects)
- `tags` — space-separated list of technology/skill tags (e.g., `"#react #typescript #nodejs"`). The frontend splits by whitespace to render individual tags.
- `highlight` — boolean indicating whether the project should be highlighted on the frontend (displayed with a star)

## File Format

Posts use the `.mdx` extension (MDX format).
