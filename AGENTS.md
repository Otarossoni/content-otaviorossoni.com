# AGENTS.md

## Repository Purpose

This repository stores the content for [otaviorossoni.com](https://otaviorossoni.com) — a multilingual blog with posts in Portuguese (`pt/`), English (`en/`), and Spanish (`es/`).

## Directory Structure

```
blog/
  pt/   # Portuguese posts
  en/   # English posts
  es/   # Spanish posts
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

## File Format

Posts use the `.mdx` extension (MDX format).
