# content-otaviorossoni.com

Content repository for [otaviorossoni.com](https://otaviorossoni.com).

## Structure

```
blog/
  pt/   # Portuguese posts
  en/   # English posts
  es/   # Spanish posts
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
