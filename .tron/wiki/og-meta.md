---
type: convention
description: Open Graph / Twitter meta convention for all site HTML
---

Every page `<head>`, inserted after `</title>`:
- `name="description"` (only if absent)
- `og:site_name` `og:type=website` `og:title` `og:description` `og:url` `og:image`
- `twitter:card` `twitter:title` `twitter:description` `twitter:image`

`og:image` sources:
- app landing/legal pages -> `assets/logos/<app>.*` (1024x1024) + `twitter:card=summary`
- generic pages -> `assets/img/truebloom-watercolor-hero.png` (1536x1024) + `summary_large_image`

Base URL `https://truebloom.ltd` (CNAME). `depends-on:: [[assets]]`
